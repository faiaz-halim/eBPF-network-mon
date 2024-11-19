Generating Traffic and Observability Report...
# Cilium Traffic and Observability Report
## Generated at: Tue Nov 19 10:47:08 AM NST 2024

## 1. Network Policy Status
```yaml
apiVersion: v1
items: []
kind: List
metadata:
  resourceVersion: ""
```

## 2. Hubble Flow Analysis
### 2.1 Flow Summary
```
Traffic Patterns:
- Flow Categories:
  - DNS Queries: 80
  - HTTP Flows: 0
  - TCP Connections: 620
  - Denied Flows: 50
  - Total Flows: 700
```

### 2.2 Notable Flows
```
HTTP Interactions:

Denied Flows:
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46388 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54496 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54494 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46320 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:47028 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46458 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54628 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52540 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46408 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52462 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52402 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46378 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54544 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54542 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-xwwgs:47000 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54562 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-b5j9k:52420 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-b5j9k:52410 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-xwwgs:46946 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-r9zh4:40808 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54638 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54618 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-ccmlh:46400 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-b5j9k:52494 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54514 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:55.895: cilium-demo/backend-stresser-567cdf7978-lmkfq:58232 (ID:35908) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:55.895: cilium-demo/backend-stresser-567cdf7978-bwbdl:43884 (ID:9677) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:59.974: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:59.991: cilium-demo/backend-stresser-567cdf7978-k4fnt:35892 (ID:29649) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:01.015: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:02.039: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:03.063: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:04.087: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:05.111: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:07.159: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:11.191: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:19.447: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:22.520: cilium-demo/traffic-generator:53842 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:35.832: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:08.087: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:29.587: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:30.615: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:31.640: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:32.663: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:33.687: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:34.711: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:36.759: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:40.791: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:49.047: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:17:05.431: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
```

### 2.3 Service Communication Matrix
| Source | Destination | Protocol | Status |
|--------|-------------|-----------|---------|
| Nov 19 14:14:18.123: cilium-demo/load-tester-67bc49c98c-xwwgs:36670 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.124: cilium-demo/load-tester-67bc49c98c-xwwgs:36437 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.124: cilium-demo/load-tester-67bc49c98c-xwwgs:48684 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.125: cilium-demo/load-tester-67bc49c98c-vcqhs:52295 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.125: cilium-demo/load-tester-67bc49c98c-vcqhs:54562 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.125: cilium-demo/load-tester-67bc49c98c-vcqhs:54566 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.126: cilium-demo/load-tester-67bc49c98c-xwwgs:46952 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.126: cilium-demo/load-tester-67bc49c98c-xwwgs:46960 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.126: cilium-demo/load-tester-67bc49c98c-vcqhs:58330 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.126: cilium-demo/load-tester-67bc49c98c-vcqhs:46252 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-vcqhs:37526 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-vcqhs:50259 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-xwwgs:47776 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-xwwgs:46964 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-vcqhs:56790 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-vcqhs:54580 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-xwwgs:46968 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-vcqhs:54588 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.128: cilium-demo/load-tester-67bc49c98c-vcqhs:59675 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.128: cilium-demo/load-tester-67bc49c98c-vcqhs:54596 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.128: cilium-demo/load-tester-67bc49c98c-xwwgs:35588 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-xwwgs:33487 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-xwwgs:53846 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-xwwgs:46970 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-vcqhs:54602 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-vcqhs:54618 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-xwwgs:60852 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.130: cilium-demo/load-tester-67bc49c98c-xwwgs:46972 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.130: cilium-demo/load-tester-67bc49c98c-xwwgs:55939 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.130: cilium-demo/load-tester-67bc49c98c-xwwgs:55225 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.130: cilium-demo/load-tester-67bc49c98c-vcqhs:54622 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.130: cilium-demo/load-tester-67bc49c98c-xwwgs:46974 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.130: cilium-demo/load-tester-67bc49c98c-xwwgs:46990 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-xwwgs:46992 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-xwwgs:47000 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-xwwgs:47014 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-ccmlh:60298 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-endpoint FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-xwwgs:47028 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.130: cilium-demo/load-tester-67bc49c98c-vcqhs:54628 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.132: cilium-demo/load-tester-67bc49c98c-xwwgs:47032 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-vcqhs:54638 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.654: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:18.655: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:20.012: cilium-demo/backend-stresser-567cdf7978-bwbdl:59076 (ID:9677) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:20.012: cilium-demo/backend-stresser-567cdf7978-bwbdl:59076 (ID:9677) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-endpoint FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:20.013: cilium-demo/backend-stresser-567cdf7978-bwbdl:43884 (ID:9677) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:20.014: cilium-demo/backend-stresser-567cdf7978-lmkfq:34027 (ID:35908) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:20.014: cilium-demo/backend-stresser-567cdf7978-lmkfq:34027 (ID:35908) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-endpoint FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:24.107: cilium-demo/backend-stresser-567cdf7978-k4fnt:44211 (ID:29649) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-endpoint FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:20.014: cilium-demo/backend-stresser-567cdf7978-lmkfq:58232 (ID:35908) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.111: cilium-demo/backend-stresser-567cdf7978-bwbdl:43884 (ID:9677) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:47028 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:47032 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:21.592: cilium-demo/traffic-generator:53842 (ID:780) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:47014 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46920 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46914 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46974 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.111: cilium-demo/backend-stresser-567cdf7978-lmkfq:58232 (ID:35908) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46968 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46992 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46912 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54562 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46964 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46972 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46990 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54580 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46922 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46946 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:47000 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54588 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46894 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54532 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46896 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:26.711: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54542 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46952 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:35.583: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46960 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54544 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:35.586: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54628 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-xwwgs:46970 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:35.927: 10.244.0.82:48244 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54550 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:31.191: cilium-demo/backend-stresser-567cdf7978-bwbdl:43884 (ID:9677) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52410 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52420 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52344 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54602 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52494 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52506 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52438 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54522 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52346 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52512 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52446 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54596 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:47014 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54622 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46968 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46992 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54494 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46922 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46912 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46964 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52402 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54496 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52462 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52540 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46972 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54566 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52376 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-b5j9k:52392 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54508 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46990 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.464: cilium-demo/load-tester-67bc49c98c-b5j9k:52362 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.464: cilium-demo/load-tester-67bc49c98c-b5j9k:52368 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46946 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54524 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:47000 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54514 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:39.817: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46896 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54618 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:41.642: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:18.126: cilium-demo/load-tester-67bc49c98c-ccmlh:57785 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46952 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-vcqhs:54638 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:41.642: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-ccmlh:43752 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:50.432: cilium-demo/prometheus-b5664c7bf-7b85r:37552 (ID:7179) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-ccmlh:46390 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-ccmlh:51383 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46960 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:31.191: cilium-demo/backend-stresser-567cdf7978-lmkfq:58232 (ID:35908) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52446 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.127: cilium-demo/load-tester-67bc49c98c-ccmlh:45065 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:33.879: cilium-demo/traffic-generator:53842 (ID:780) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52438 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46970 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52392 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54542 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46894 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.128: cilium-demo/load-tester-67bc49c98c-ccmlh:58120 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52376 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54544 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:47028 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.128: cilium-demo/load-tester-67bc49c98c-ccmlh:46400 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52368 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54562 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:47032 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.128: cilium-demo/load-tester-67bc49c98c-ccmlh:47238 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52362 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54532 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52524 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-xwwgs:46920 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54522 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52540 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.128: cilium-demo/load-tester-67bc49c98c-ccmlh:33786 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:37.464: cilium-demo/load-tester-67bc49c98c-xwwgs:46914 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54550 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52462 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52402 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.464: cilium-demo/load-tester-67bc49c98c-xwwgs:46974 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52328 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-ccmlh:44999 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54602 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52478 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:39.511: cilium-demo/backend-stresser-567cdf7978-bwbdl:43884 (ID:9677) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52512 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54494 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-ccmlh:46408 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52506 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:47032 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52430 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-ccmlh:47373 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54496 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52346 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:47014 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52344 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54596 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-ccmlh:53728 (ID:27393) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46990 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54566 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46970 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54622 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.129: cilium-demo/load-tester-67bc49c98c-ccmlh:46424 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:47028 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54514 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46894 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54618 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.130: cilium-demo/load-tester-67bc49c98c-ccmlh:46428 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46922 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54638 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46974 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54628 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.130: cilium-demo/load-tester-67bc49c98c-ccmlh:46442 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46972 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54580 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-vcqhs:54588 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46960 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.464: cilium-demo/load-tester-67bc49c98c-vcqhs:54508 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46992 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-ccmlh:46458 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.464: cilium-demo/load-tester-67bc49c98c-vcqhs:54524 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46920 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:39.511: cilium-demo/backend-stresser-567cdf7978-lmkfq:58232 (ID:35908) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46952 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:50.263: cilium-demo/traffic-generator:53842 (ID:780) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46896 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54532 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46968 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54524 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46964 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54508 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46914 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:43.863: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54496 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:46912 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.197: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-ccmlh:46474 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54494 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.198: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-ccmlh:60298 (ID:27393) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-xwwgs:47000 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-b5j9k:52494 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54566 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-xwwgs:46946 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-b5j9k:52420 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-b5j9k:52410 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-ccmlh:46478 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54628 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54544 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.131: cilium-demo/load-tester-67bc49c98c-ccmlh:46494 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54542 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54622 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:18.132: cilium-demo/load-tester-67bc49c98c-ccmlh:46504 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54596 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54588 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:24.107: cilium-demo/backend-stresser-567cdf7978-k4fnt:44211 (ID:29649) | kube-system/coredns-7c65d6cfc9-lz9bx:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54580 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:54.871: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:55.895: cilium-demo/backend-stresser-567cdf7978-bwbdl:43884 (ID:9677) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:56.919: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:56.919: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54522 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:59.974: cilium-demo/metric-test:33129 (ID:4630) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:59.974: cilium-demo/metric-test:33129 (ID:4630) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-endpoint FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54602 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:59.974: cilium-demo/metric-test:44480 (ID:4630) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:24.107: cilium-demo/backend-stresser-567cdf7978-k4fnt:35892 (ID:29649) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54550 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46494 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54638 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:04.817: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:15:05.111: cilium-demo/metric-test:44480 (ID:4630) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46378 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:05.928: 10.244.0.82:48244 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46408 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54562 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:08.210: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:15:08.211: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46458 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54618 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54514 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:55.895: cilium-demo/backend-stresser-567cdf7978-lmkfq:58232 (ID:35908) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:11.191: cilium-demo/metric-test:44480 (ID:4630) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:11.643: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:15:11.643: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46474 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46400 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:18.657: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46442 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:18.658: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:15:19.447: cilium-demo/metric-test:44480 (ID:4630) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:19.959: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46478 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46342 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46390 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46424 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46320 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:20.433: cilium-demo/prometheus-b5664c7bf-7b85r:37552 (ID:7179) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46388 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:22.520: cilium-demo/traffic-generator:53842 (ID:780) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46504 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:27.127: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46338 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46360 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:27.127: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46428 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46324 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46350 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:25.303: cilium-demo/load-tester-67bc49c98c-ccmlh:46362 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:29.207: cilium-demo/backend-stresser-567cdf7978-k4fnt:35892 (ID:29649) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:29.818: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:15:35.510: 10.244.0.82:48244 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:35.287: cilium-demo/backend-stresser-567cdf7978-k4fnt:35892 (ID:29649) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46378 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46474 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46400 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46442 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:35.583: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46478 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:35.585: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46360 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:35.832: cilium-demo/metric-test:44480 (ID:4630) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46428 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46342 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46390 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46424 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46320 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46388 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46504 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:41.644: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46324 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46350 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46362 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46338 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46408 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.463: cilium-demo/load-tester-67bc49c98c-ccmlh:46458 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:37.464: cilium-demo/load-tester-67bc49c98c-ccmlh:46494 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:41.645: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:43.607: cilium-demo/backend-stresser-567cdf7978-k4fnt:35892 (ID:29649) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:43.868: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46338 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:45.047: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46424 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:46.435: cilium-demo/prometheus-b5664c7bf-7b85r:37552 (ID:7179) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46390 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:53.252: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46342 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:53.253: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46428 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:54.818: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46360 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46458 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46408 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:56.823: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46378 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:15:56.823: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:16:05.929: 10.244.0.82:48244 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46362 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46350 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46324 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46478 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46442 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46494 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46474 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46504 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46388 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:16:08.087: cilium-demo/metric-test:44480 (ID:4630) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46320 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-ccmlh:46400 (ID:27393) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:14:59.991: cilium-demo/backend-stresser-567cdf7978-k4fnt:35892 (ID:29649) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:16:08.264: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:08.265: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:10.135: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:16:11.646: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:11.646: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:16.437: cilium-demo/prometheus-b5664c7bf-7b85r:37552 (ID:7179) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:18.661: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:18.662: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:19.819: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:27.031: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:16:27.031: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:16:29.586: cilium-demo/traffic-generator:60961 (ID:780) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-overlay FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:16:29.586: cilium-demo/traffic-generator:60961 (ID:780) | kube-system/coredns-7c65d6cfc9-6zdfl:53 (ID:32003) to-endpoint FORWARDED (UDP) | UDP | ALLOWED |
| Nov 19 14:16:29.586: cilium-demo/traffic-generator:53956 (ID:780) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:16:29.865: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:16:30.467: cilium-demo/prometheus-b5664c7bf-7b85r:37552 (ID:7179) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:35.223: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:16:35.583: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:35.586: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:35.929: 10.244.0.82:48244 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:36.759: cilium-demo/traffic-generator:53956 (ID:780) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:16:41.648: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:41.648: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:43.349: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:16:44.819: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:49.047: cilium-demo/traffic-generator:53956 (ID:780) | cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) to-overlay FORWARDED (TCP Flags: SYN) | TCP | ALLOWED |
| Nov 19 14:16:53.308: 10.244.0.82:48220 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:53.309: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:54648 (ID:34272) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:16:56.728: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-overlay FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:16:56.728: cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:39030 (ID:34272) | cilium-demo/prometheus-b5664c7bf-7b85r:9090 (ID:7179) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:17:00.311: 10.244.0.82:40632 (world) | cilium-demo/grafana-59d46d755-rh2jl:3000 (ID:7249) to-endpoint FORWARDED (TCP Flags: ACK) | TCP | ALLOWED |
| Nov 19 14:17:00.468: cilium-demo/prometheus-b5664c7bf-7b85r:37552 (ID:7179) | 172.19.0.7:6443 (kube-apiserver) to-stack FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |
| Nov 19 14:17:05.931: 10.244.0.82:48244 (remote-node) | cilium-demo/prometheus-adapter-fbd8fc98-jxs4w:6443 (ID:34272) to-endpoint FORWARDED (TCP Flags: ACK, PSH) | TCP | ALLOWED |

### 2.4 Policy Enforcement Details
```
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46388 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54496 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54494 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46320 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-xwwgs:47028 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46458 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54628 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52540 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46408 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52462 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-b5j9k:52402 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-ccmlh:46378 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54544 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.847: cilium-demo/load-tester-67bc49c98c-vcqhs:54542 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-xwwgs:47000 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54562 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-b5j9k:52420 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-b5j9k:52410 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-xwwgs:46946 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-r9zh4:40808 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54638 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54618 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-ccmlh:46400 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-b5j9k:52494 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:53.848: cilium-demo/load-tester-67bc49c98c-vcqhs:54514 (ID:27393) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:55.895: cilium-demo/backend-stresser-567cdf7978-lmkfq:58232 (ID:35908) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:55.895: cilium-demo/backend-stresser-567cdf7978-bwbdl:43884 (ID:9677) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:59.974: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:14:59.991: cilium-demo/backend-stresser-567cdf7978-k4fnt:35892 (ID:29649) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:01.015: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:02.039: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:03.063: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:04.087: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:05.111: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:07.159: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:11.191: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:19.447: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:22.520: cilium-demo/traffic-generator:53842 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:15:35.832: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:08.087: cilium-demo/metric-test:44480 (ID:4630) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:29.587: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:30.615: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:31.640: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:32.663: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:33.687: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:34.711: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:36.759: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:40.791: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:16:49.047: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
Nov 19 14:17:05.431: cilium-demo/traffic-generator:53956 (ID:780) <> cilium-demo/backend-648859cbf9-q2lgx:80 (ID:53775) policy-verdict:none INGRESS DENIED (TCP Flags: SYN)
```

## 3. HTTP Request Metrics
```json
```

## 4. Policy Drops
```json
```

## 5. HPA Status
```yaml
apiVersion: v1
items:
- apiVersion: autoscaling/v2
  kind: HorizontalPodAutoscaler
  metadata:
    annotations:
      kubectl.kubernetes.io/last-applied-configuration: |
        {"apiVersion":"autoscaling/v2","kind":"HorizontalPodAutoscaler","metadata":{"annotations":{},"name":"backend-hpa","namespace":"cilium-demo"},"spec":{"maxReplicas":10,"metrics":[{"object":{"describedObject":{"apiVersion":"v1","kind":"Service","name":"backend"},"metric":{"name":"http_requests_per_second"},"target":{"type":"Value","value":10}},"type":"Object"},{"resource":{"name":"cpu","target":{"averageUtilization":50,"type":"Utilization"}},"type":"Resource"},{"resource":{"name":"memory","target":{"averageUtilization":80,"type":"Utilization"}},"type":"Resource"}],"minReplicas":1,"scaleTargetRef":{"apiVersion":"apps/v1","kind":"Deployment","name":"backend"}}}
    creationTimestamp: "2024-11-19T13:58:22Z"
    labels:
      k8slens-edit-resource-version: v2
    name: backend-hpa
    namespace: cilium-demo
    resourceVersion: "53826"
    uid: df6eae41-05ec-4270-9a32-0d55fb661f0e
  spec:
    maxReplicas: 10
    metrics:
    - object:
        describedObject:
          apiVersion: v1
          kind: Service
          name: backend
        metric:
          name: http_requests_per_second
        target:
          type: Value
          value: "10"
      type: Object
    - resource:
        name: cpu
        target:
          averageUtilization: 50
          type: Utilization
      type: Resource
    - resource:
        name: memory
        target:
          averageUtilization: 80
          type: Utilization
      type: Resource
    minReplicas: 1
    scaleTargetRef:
      apiVersion: apps/v1
      kind: Deployment
      name: backend
  status:
    conditions:
    - lastTransitionTime: "2024-11-19T13:58:37Z"
      message: recommended size matches current size
      reason: ReadyForNewScale
      status: "True"
      type: AbleToScale
    - lastTransitionTime: "2024-11-19T13:58:37Z"
      message: the HPA was able to successfully calculate a replica count from memory
        resource utilization (percentage of request)
      reason: ValidMetricFound
      status: "True"
      type: ScalingActive
    - lastTransitionTime: "2024-11-19T13:58:37Z"
      message: the desired count is within the acceptable range
      reason: DesiredWithinRange
      status: "False"
      type: ScalingLimited
    currentMetrics:
    - type: ""
    - resource:
        current:
          averageUtilization: 0
          averageValue: "0"
        name: cpu
      type: Resource
    - resource:
        current:
          averageUtilization: 10
          averageValue: "13426688"
        name: memory
      type: Resource
    currentReplicas: 1
    desiredReplicas: 1
kind: List
metadata:
  resourceVersion: ""
```

## 6. Service Endpoints
```
Frontend Service:
NAME       ENDPOINTS         AGE
frontend   10.244.1.125:80   5h56m

Backend Service:
NAME      ENDPOINTS        AGE
backend   10.244.4.20:80   5h56m
```

## 7. Pod Status
```
NAME                                READY   STATUS    RESTARTS   AGE
backend-648859cbf9-q2lgx            1/1     Running   0          28m
frontend-6d6ccf4d7c-5pd5q           1/1     Running   0          28m
grafana-59d46d755-rh2jl             1/1     Running   0          5h48m
metric-test                         1/1     Running   0          5h56m
prometheus-adapter-fbd8fc98-jxs4w   1/1     Running   0          5h48m
prometheus-b5664c7bf-7b85r          1/1     Running   0          5h56m
traffic-generator                   1/1     Running   0          4h40m
```

