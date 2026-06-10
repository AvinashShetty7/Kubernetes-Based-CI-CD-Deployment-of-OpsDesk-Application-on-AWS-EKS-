# Kubernetes CI/CD Deployment on Amazon EKS

## Project Overview

This project demonstrates a complete cloud-native deployment workflow using Amazon EKS, Docker, Kubernetes, Helm, and GitHub Actions.

The primary focus of this project is implementing DevOps best practices by automating application build, containerization, deployment, and orchestration on a managed Kubernetes cluster.

---

## Architecture

![Architecture](./diagrams/architecture.png)

---

## Key DevOps Highlights

- Amazon EKS Cluster Deployment
- Kubernetes Workload Management
- Docker Containerization
- GitHub Actions CI/CD Pipeline
- Helm Chart Deployment
- ConfigMap and Secret Management
- Rolling Updates
- Service Discovery
- Container Orchestration
- Cloud-Native Deployment

---

## Deployment Workflow

```text
Developer
    │
    ▼
GitHub Repository
    │
    ▼
GitHub Actions
    │
    ├── Build Docker Images
    ├── Push Images to Registry
    └── Deploy to EKS
    │
    ▼
Amazon EKS Cluster
    │
    ▼
Helm Charts
    │
    ▼
Kubernetes Deployments
    │
    ▼
Services & Pods
```

---

## Technology Stack

### Cloud Platform

- AWS EKS
- AWS EC2
- AWS IAM
- AWS VPC

### Containerization

- Docker

### Orchestration

- Kubernetes
- Helm

### CI/CD

- GitHub Actions

### Version Control

- Git
- GitHub

---

## Kubernetes Resources

### Workloads

- Backend Deployment
- Frontend Deployment

### Networking

- Kubernetes Services
- LoadBalancer Service
- ClusterIP Service

### Configuration

- ConfigMaps
- Secrets

### Deployment Strategy

- Rolling Updates
- Replica Management

---

## CI/CD Pipeline

The deployment process is fully automated using GitHub Actions.

### Pipeline Stages

1. Source Code Checkout
2. Docker Image Build
3. Docker Image Push
4. Kubernetes Authentication
5. Helm Upgrade/Install
6. Deployment Verification

---



---

## Skills Demonstrated

- Kubernetes Administration
- Amazon EKS Management
- Docker Containerization
- Helm Package Management
- CI/CD Pipeline Automation
- GitHub Actions
- Cloud-Native Deployments
- Kubernetes Networking
- Configuration Management
- DevOps Best Practices

---

## Learning Outcomes

Through this project, I gained hands-on experience with:

- Deploying applications on Amazon EKS
- Building automated CI/CD pipelines
- Managing Kubernetes resources
- Helm-based application deployment
- Container lifecycle management
- Cloud-native application delivery
- Infrastructure automation
- Deployment troubleshooting

---

## Future Enhancements

- ArgoCD GitOps
- Prometheus Monitoring
- Grafana Dashboards
- Horizontal Pod Autoscaler
- AWS Load Balancer Controller
- Ingress Controller
- Blue-Green Deployment
- Canary Releases

---

## Author

**Avinash Shetty**

DevOps Engineer | AWS | Kubernetes | Docker | Terraform | GitHub Actions
