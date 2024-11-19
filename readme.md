# Dynamic Network Traffic Monitoring and Scaling Using eBPF

## Overview

This project implements an advanced network monitoring and dynamic scaling system using eBPF technology in a Kubernetes environment. It leverages Cilium for eBPF-powered networking, providing real-time traffic visibility and automated scaling based on network metrics and resource utilization.

## Key Features

1. Real-time network flow monitoring using eBPF
2. Dynamic scaling based on traffic patterns and resource metrics
3. Network policy enforcement and monitoring
4. Comprehensive traffic visualization
5. Automated load testing and reporting

## Core Infrastructure

1. Kubernetes 1.31 cluster (kind)
2. Cilium 1.16.3 with eBPF
3. Hubble for flow visibility

## Monitoring Stack

1. Prometheus for metrics storage
2. Custom Prometheus Adapter
3. Grafana for visualization

## Application Layer

1. Frontend service
2. Backend service
3. Load testing suite

## Prerequisites

Docker
Kind
kubectl
Helm v3
curl
jq

# Quick Start

## Install cluster:

```
make up-cilium
```

## Deploy the environment:

```
make deploy
make port-forward
```

## Run tests:

```
make test
```

## Generate and view reports:

```
make view-report
```
