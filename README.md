# Microservices Kubernetes Deployment using Minikube

## Objective

The objective of this project is to deploy a containerized microservices-based application using Kubernetes and Minikube. The deployment demonstrates Kubernetes concepts such as Deployments, Services, Inter-Service Communication, Ingress Configuration, and cluster validation.

---

# Technologies Used

- Kubernetes
- Minikube
- Docker Desktop
- kubectl
- NGINX Containers
- macOS Terminal

---

# Application Architecture

The application consists of four microservices:

| Service Name | Purpose | Port |
|---|---|---|
| User Service | Handles user-related requests | 3000 |
| Product Service | Handles product-related requests | 3001 |
| Order Service | Handles order-related requests | 3002 |
| Gateway Service | Entry point and routing service | 3003 |

---

# Kubernetes Components Implemented

## Deployments
Created Kubernetes Deployment manifests for:
- User Service
- Product Service
- Order Service
- Gateway Service

Each deployment includes:
- Labels and selectors
- Resource requests and limits
- Environment variables
- Liveness probes
- Readiness probes

---

## Services
Created ClusterIP services for:
- User Service
- Product Service
- Order Service
- Gateway Service

These services enable:
- Internal Kubernetes DNS communication
- Service discovery
- Pod-to-pod communication

---

## Ingress Configuration
Implemented Kubernetes Ingress with path-based routing:

| Path | Service |
|---|---|
| /api/users | User Service |
| /api/products | Product Service |
| /api/orders | Order Service |
| / | Gateway Service |

Ingress controller was enabled using Minikube addons.

---

# Folder Structure

```text
submission/
├── deployments/
├── services/
├── ingress/
├── screenshots/
└── README.md
