# Kubernetes GitOps Configuration

Infrastructure as Code for all Kubernetes deployments managed by Flux CD.

## Repository Structure

```plaintext
.
├── clusters/                # Application workloads
│   ├── production/         # Production environment
│   │   ├── textsage/      # TextSage application
│   │   └── swing-analyzer/ # Swing Analyzer application
│   └── staging/           # Staging environment
└── infrastructure/        # Shared infrastructure
    ├── monitoring/       # Prometheus & Grafana
    ├── ingress-nginx/   # Ingress controller
    ├── cert-manager/    # Certificate management
    └── sealed-secrets/  # Secret encryption
```

## Applications

### TextSage
Open-source document processing and analysis application.

### Swing Analyzer
Private golf swing analysis application.

## Infrastructure Components
- **Monitoring**: Prometheus and Grafana for observability
- **Ingress-Nginx**: Kubernetes ingress controller
- **Cert-Manager**: Automatic TLS certificate management
- **Sealed-Secrets**: Secure secret management

## Usage
Changes to the main branch are automatically synchronized with the cluster by Flux CD.
