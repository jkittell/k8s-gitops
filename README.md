# k8s-gitops

GitOps repository for managing Kubernetes clusters.

## Clusters
- `local`: Rancher Desktop development environment
- `staging`: DigitalOcean staging environment
- `production`: DigitalOcean production environment

## Prerequisites
- flux
- kubectl
- kubeseal
- helm

## Setup
1. Clone repository
2. Bootstrap Flux
3. Wait for reconciliation

## Directory Structure
- `/clusters`: Cluster-specific configurations
  - `/local`: Local development
  - `/staging`: Staging environment
  - `/production`: Production environment

## Infrastructure
- cert-manager
- ingress-nginx
- monitoring (Prometheus/Grafana)
- sealed-secrets