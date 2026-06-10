# Kubernetes-Based CI/CD Deployment of OpsDesk Application on AWS EKS

## Overview

This project demonstrates a complete cloud-native DevOps workflow for deploying a full-stack **OpsDesk Ticket Management Application** on **Amazon EKS** using **Kubernetes, Docker, Helm, GitHub Actions, and ArgoCD**.

The primary objective of this project is to implement modern DevOps practices including containerization, CI/CD automation, Kubernetes orchestration, and GitOps-based continuous delivery.

---

## Architecture

<img width="1536" height="1024" alt="archfork8s" src="https://github.com/user-attachments/assets/66c4dfa0-f07a-4287-8979-86fbdfc1d979" />


---

## Technology Stack

| Category | Technologies |
|-----------|-------------|
| Cloud Platform | AWS EKS |
| Containerization | Docker |
| Orchestration | Kubernetes |
| CI/CD | GitHub Actions |
| Package Management | Helm |
| GitOps | ArgoCD |
| Ingress Controller | NGINX Ingress |
| Frontend | React.js |
| Backend | Node.js, Express.js |
| Database | MongoDB |

---

## DevOps Workflow

```text
Developer
    |
    ▼
GitHub Repository
    |
    ▼
GitHub Actions CI Pipeline
    |
    ├── Build Frontend Docker Image
    ├── Build Backend Docker Image
    ├── Push Images to Docker Registry
    └── Update Helm Values with New Image Tags
    |
    ▼
Git Repository (Helm Charts)
    |
    ▼
ArgoCD
    |
    ▼
Amazon EKS Cluster
    |
    ▼
Kubernetes Deployments
    |
    ▼
NGINX Ingress
    |
    ▼
End Users
```

---

## Key DevOps Features

### Containerization

- Containerized frontend and backend applications using Docker.
- Created production-ready Dockerfiles.
- Built immutable Docker images for consistent deployments.

### Kubernetes Orchestration

- Deployed applications on Amazon EKS.
- Implemented Kubernetes Deployments and Services.
- Configured ConfigMaps for application configuration.
- Managed ingress traffic using NGINX Ingress Controller.

### CI/CD Automation

Implemented a fully automated CI pipeline using GitHub Actions:

- Automatic pipeline trigger on code push.
- Docker image build automation.
- Container image publishing to registry.
- Helm chart updates with latest image tags.
- Continuous deployment workflow integration.

### Helm-Based Deployment

- Created reusable Helm charts.
- Parameterized deployment configurations.
- Managed Kubernetes resources through templates.
- Simplified release management.

### GitOps with ArgoCD

- Continuous monitoring of Git repositories.
- Automatic synchronization of cluster state.
- Deployment automation without manual intervention.
- Desired state management using GitOps principles.

---

## AWS Services Used

### Amazon EKS

Managed Kubernetes cluster hosting application workloads.

### EC2 Worker Nodes

Compute infrastructure for running Kubernetes Pods.

### Elastic Load Balancer

External traffic distribution to application services.

### IAM

Role-based access control and permissions management.

### VPC Networking

Secure networking environment for cluster resources.

---

## Kubernetes Resources

### Deployments

- Frontend Deployment
- Backend Deployment

### Services

- Frontend Service
- Backend Service

### ConfigMaps

- Application configuration management

### Ingress

- NGINX Ingress Controller
- External traffic routing

---

## Repository Structure

```text
TICKETDESKAPP
│
├── .github
│   └── workflows
│       └── ci.yaml
│
├── backend
│   ├── Dockerfile
│   └── source code
│
├── frontend
│   ├── Dockerfile
│   └── source code
│
├── helm
│   └── ticketapp-chart
│       ├── templates
│       ├── Chart.yaml
│       ├── values.yaml
│       └── .helmignore
│
├── k8s
│   └── manifests
│
└── README.md
```

---

## CI/CD Pipeline Stages

### 1. Source Code Checkout

Fetch latest application source code from GitHub.

### 2. Docker Image Build

Build frontend and backend Docker images.

### 3. Push Images

Push versioned images to Docker Registry.

### 4. Helm Chart Update

Update image tags in Helm values file.

### 5. GitOps Deployment

ArgoCD detects Helm changes and automatically synchronizes deployments to Amazon EKS.

---

## Skills Demonstrated

- Kubernetes Administration
- Amazon EKS
- Docker Containerization
- GitHub Actions CI/CD
- GitOps with ArgoCD
- Helm Chart Development
- Kubernetes Networking
- NGINX Ingress Controller
- Cloud-Native Application Deployment
- Continuous Integration
- Continuous Delivery
- DevOps Automation
- Container Orchestration

---

## Future Enhancements

- Terraform-based EKS provisioning
- Prometheus Monitoring
- Grafana Dashboards
- AWS CloudWatch Integration
- Horizontal Pod Autoscaler (HPA)
- Kubernetes Secret Management
- Blue-Green Deployments
- Canary Releases
- Multi-Environment Deployment Strategy

---

## Results

✅ Automated CI/CD Pipeline

✅ Dockerized Microservice Deployment

✅ GitOps-Based Continuous Delivery

✅ Kubernetes Workload Management

✅ Scalable Cloud-Native Architecture

✅ Production-Ready EKS Deployment

---

## Author

**Avinash Shetty**

DevOps Engineer | AWS | Kubernetes | Docker | Helm | GitHub Actions | ArgoCD
