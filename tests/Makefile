.PHONY: deploy test report clean

deploy:
	cilium install --version 1.16.3
	cilium status --wait
	kubectl apply -f manifest.yaml
	cilium hubble enable --ui --relay
	kubectl wait --for=condition=ready pod -l app=frontend -n cilium-demo --timeout=120s
	kubectl wait --for=condition=ready pod -l app=backend -n cilium-demo --timeout=120s
	kubectl wait --for=condition=ready pod -l app=prometheus -n cilium-demo --timeout=120s
	kubectl wait --for=condition=ready pod -l app=grafana -n cilium-demo --timeout=120s
	kubectl wait --for=condition=ready pod -l name=prometheus-adapter -n cilium-demo --timeout=120s

wait-for-metrics:
	@echo "Waiting for metrics API to become available..."
	@for i in $$(seq 1 10); do \
		echo "Attempt $$i..."; \
		if kubectl get --raw "/apis/custom.metrics.k8s.io/v1beta1" > /dev/null 2>&1; then \
			echo "Metrics API is available!"; \
			break; \
		fi; \
		sleep 10; \
	done

debug-metrics:
	@echo "Checking Prometheus Adapter logs..."
	kubectl logs -n cilium-demo -l name=prometheus-adapter
	@echo "\nChecking available metrics in Prometheus..."
	kubectl port-forward -n cilium-demo svc/prometheus 9090:9090 > /dev/null 2>&1 & \
	sleep 5 && \
	curl -s 'http://localhost:9090/api/v1/query?query=http_requests_total' | jq .
	@echo "\nChecking Hubble metrics status..."
	hubble status
	@echo "\nChecking Hubble metrics..."
	hubble observe

verify-metrics:
	@echo "Checking if Prometheus is collecting Cilium metrics..."
	kubectl port-forward -n cilium-demo svc/prometheus 9090:9090 > /dev/null 2>&1 & \
	sleep 5 && \
	curl -s 'http://localhost:9090/api/v1/query?query=http_requests_total' | jq .
	@echo "\nChecking if metrics are available through custom metrics API..."
	kubectl get --raw "/apis/custom.metrics.k8s.io/v1beta1" | jq .
	@echo "\nChecking specific metric availability..."
	kubectl get --raw "/apis/custom.metrics.k8s.io/v1beta1/namespaces/cilium-demo/services/backend/http_requests_per_second" || true
	@echo "\nChecking HPA status..."
	kubectl describe hpa backend-hpa -n cilium-demo

test: port-forward traffic
	hubble observe --namespace cilium-demo

port-forward:
	cilium hubble port-forward&
	cilium hubble ui&

traffic:
	@echo "Generating test traffic..."
	@for i in $$(seq 1 50); do \
		echo "Request $$i: Normal traffic"; \
		kubectl exec -n cilium-demo deployment/frontend -- curl -s -H "X-Ratelimit: true" http://backend/api; \
		sleep 1; \
		MOD_FIVE=$$(( $$i % 5 )); \
		if [ $$MOD_FIVE -eq 0 ]; then \
			echo "Request $$i: Testing rate limit..."; \
			for j in $$(seq 1 15); do \
				kubectl exec -n cilium-demo deployment/frontend -- curl -s -H "X-Ratelimit: true" http://backend/api; \
			done; \
			sleep 2; \
		fi; \
		MOD_SEVEN=$$(( $$i % 7 )); \
		if [ $$MOD_SEVEN -eq 0 ]; then \
			echo "Request $$i: Testing denied path..."; \
			kubectl exec -n cilium-demo deployment/frontend -- curl -s -H "X-Ratelimit: true" http://backend/forbidden; \
		fi; \
		MOD_THREE=$$(( $$i % 3 )); \
		if [ $$MOD_THREE -eq 0 ]; then \
			echo "Request $$i: Testing without rate limit header..."; \
			kubectl exec -n cilium-demo deployment/frontend -- curl -s http://backend/api; \
		fi; \
	done

continuous-traffic:
	@echo "Starting continuous traffic generation (Ctrl+C to stop)..."
	@while true; do \
		$(MAKE) traffic; \
		sleep 5; \
	done

test-cpu-burst:
	@echo "Deploying CPU load test pods..."
	kubectl apply -f load.yaml
	@echo "Waiting for CPU tester pods to be ready..."
	kubectl wait --for=condition=ready pod -l app=load-tester -n cilium-demo --timeout=60s || true
	kubectl wait --for=condition=ready pod -l app=backend-stresser -n cilium-demo --timeout=60s || true
	@echo "CPU load test started. Use 'make monitor-cpu-test' to watch the results"

monitor-cpu-test:
	@echo "Monitoring system load..."
	watch 'echo "=== HPA Status ==="; \
	      kubectl get hpa -n cilium-demo; \
	      echo "\n=== Backend Pods ==="; \
	      kubectl get pods -l app=backend -n cilium-demo; \
	      echo "\n=== Resource Usage ==="; \
	      kubectl top pods -n cilium-demo -l app=backend --sort-by=cpu; \
	      echo "\n=== Load Test Pods ==="; \
	      kubectl get pods -l app=load-tester -n cilium-demo; \
	      kubectl get pods -l app=backend-stresser -n cilium-demo; \
	      echo "\n=== Recent Scaling Events ==="; \
	      kubectl get events -n cilium-demo --sort-by=.metadata.creationTimestamp | grep "scale" | tail -5'

stop-cpu-test:
	@echo "Stopping CPU load test..."
	kubectl delete -f load.yaml
	@echo "CPU load test stopped"

report:
	@echo "Generating Traffic and Observability Report..." > traffic-report.md
	@echo "# Cilium Traffic and Observability Report" >> traffic-report.md
	@echo "## Generated at: `date`" >> traffic-report.md
	@echo "" >> traffic-report.md
	@echo "## 1. Network Policy Status" >> traffic-report.md
	@echo '```yaml' >> traffic-report.md
	@kubectl get cnp -n cilium-demo -o yaml >> traffic-report.md 2>/dev/null || echo "No network policies found"
	@echo '```' >> traffic-report.md
	@echo "" >> traffic-report.md
	@echo "## 2. Hubble Flow Analysis" >> traffic-report.md
	@hubble observe --namespace cilium-demo --last 100 > hubble_flows.tmp
	@echo "### 2.1 Flow Summary" >> traffic-report.md
	@echo '```' >> traffic-report.md
	@echo "Traffic Patterns:" >> traffic-report.md
	@awk 'BEGIN {dns=0; http=0; tcp=0; denied=0; total=0} \
		/coredns.*53/ {dns++} \
		/http-[request|response]/ {http++} \
		/TCP Flags:/ {tcp++} \
		/DENIED/ {denied++} \
		{total++} \
		END {print "- Flow Categories:"; \
		     print "  - DNS Queries:", dns; \
		     print "  - HTTP Flows:", http; \
		     print "  - TCP Connections:", tcp; \
		     print "  - Denied Flows:", denied; \
		     print "  - Total Flows:", total}' hubble_flows.tmp >> traffic-report.md
	@echo '```' >> traffic-report.md
	@echo "" >> traffic-report.md
	@echo "### 2.2 Notable Flows" >> traffic-report.md
	@echo '```' >> traffic-report.md
	@echo "HTTP Interactions:" >> traffic-report.md
	@grep "http-" hubble_flows.tmp >> traffic-report.md || true
	@echo "\nDenied Flows:" >> traffic-report.md
	@grep "DENIED" hubble_flows.tmp >> traffic-report.md || true
	@echo '```' >> traffic-report.md
	@echo "" >> traffic-report.md
	@echo "### 2.3 Service Communication Matrix" >> traffic-report.md
	@echo "| Source | Destination | Protocol | Status |" >> traffic-report.md
	@echo "|--------|-------------|-----------|---------|" >> traffic-report.md
	@awk 'BEGIN {FS=" -> "} \
		/->/ { \
			source=$$1; \
			dest=$$2; \
			status="ALLOWED"; \
			if ($$0 ~ /DENIED/) status="DENIED"; \
			proto="Unknown"; \
			if ($$0 ~ /UDP/) proto="UDP"; \
			if ($$0 ~ /TCP/) proto="TCP"; \
			printf "| %s | %s | %s | %s |\n", source, dest, proto, status \
		}' hubble_flows.tmp >> traffic-report.md
	@echo "" >> traffic-report.md
	@echo "### 2.4 Policy Enforcement Details" >> traffic-report.md
	@echo '```' >> traffic-report.md
	@grep "policy-verdict" hubble_flows.tmp >> traffic-report.md || true
	@echo '```' >> traffic-report.md
	@echo "" >> traffic-report.md
	@rm -f hubble_flows.tmp
	@echo "## 3. HTTP Request Metrics" >> traffic-report.md
	@echo '```json' >> traffic-report.md
	@kubectl port-forward -n cilium-demo svc/prometheus 9090:9090 > /dev/null 2>&1 & \
	PROM_PID=$$!; \
	sleep 2; \
	curl -s 'http://localhost:9090/api/v1/query?query=rate(http_requests_total[5m])' | jq . >> traffic-report.md 2>/dev/null || echo "No metrics data available";
	@echo '```' >> traffic-report.md
	@echo "" >> traffic-report.md
	@echo "## 4. Policy Drops" >> traffic-report.md
	@echo '```json' >> traffic-report.md
	@kubectl port-forward -n cilium-demo svc/prometheus 9090:9090 > /dev/null 2>&1 & \
	PROM_PID=$$!; \
	sleep 2; \
	curl -s 'http://localhost:9090/api/v1/query?query=rate(drop_count_total[5m])' | jq . >> traffic-report.md 2>/dev/null || echo "No drop metrics available";
	@echo '```' >> traffic-report.md
	@echo "" >> traffic-report.md
	@echo "## 5. HPA Status" >> traffic-report.md
	@echo '```yaml' >> traffic-report.md
	@kubectl get hpa -n cilium-demo -o yaml >> traffic-report.md 2>/dev/null || echo "No HPA found"
	@echo '```' >> traffic-report.md
	@echo "" >> traffic-report.md
	@echo "## 6. Service Endpoints" >> traffic-report.md
	@echo '```' >> traffic-report.md
	@echo "Frontend Service:" >> traffic-report.md
	@kubectl get endpoints -n cilium-demo frontend -o wide >> traffic-report.md 2>/dev/null || echo "No frontend endpoints found"
	@echo "\nBackend Service:" >> traffic-report.md
	@kubectl get endpoints -n cilium-demo backend -o wide >> traffic-report.md 2>/dev/null || echo "No backend endpoints found"
	@echo '```' >> traffic-report.md
	@echo "" >> traffic-report.md
	@echo "## 7. Pod Status" >> traffic-report.md
	@echo '```' >> traffic-report.md
	@kubectl get pods -n cilium-demo >> traffic-report.md 2>/dev/null || echo "No pods found"
	@echo '```' >> traffic-report.md
	@echo "" >> traffic-report.md
	@echo "Report generated at traffic-report.md"

view-report: report
	@if command -v glow > /dev/null; then \
		glow traffic-report.md; \
	else \
		cat traffic-report.md; \
	fi

clean:
	kubectl delete namespace cilium-demo
	pkill -f "port-forward"