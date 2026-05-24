# Microservices Kubernetes Deployment using Minikube

## Objective

Deploy and validate a microservices-based application using Kubernetes and Minikube demonstrating:
- Kubernetes Deployments
- Kubernetes Services
- Inter-service communication
- Ingress configuration
- Kubernetes networking

---

# Technologies Used

- Kubernetes
- Minikube
- Docker Desktop
- kubectl
- NGINX Containers

---

# Application Components

| Service Name | Port |
|---|---|
| User Service | 3000 |
| Product Service | 3001 |
| Order Service | 3002 |
| Gateway Service | 3003 |

---

# Kubernetes Resources Implemented

## Deployments
Implemented deployments for:
- User Service
- Product Service
- Order Service
- Gateway Service

Each deployment includes:
- Labels and selectors
- Resource requests and limits
- Liveness probes
- Readiness probes

---

## Services
Implemented ClusterIP services for:
- User Service
- Product Service
- Order Service
- Gateway Service

These services enable:
- Internal cluster communication
- Kubernetes DNS-based service discovery
- Pod-to-pod communication

---

## Ingress
Implemented Kubernetes Ingress with path-based routing.

| Path | Routed Service |
|---|---|
| /api/users | User Service |
| /api/products | Product Service |
| /api/orders | Order Service |
| / | Gateway Service |

---

# Validation Performed

- Verified Minikube cluster
- Verified running pods
- Verified services
- Tested inter-service communication
- Verified ingress controller
- Tested external service access

---

# Project Structure

```text
submission/
├── deployments/
├── services/
├── ingress/
├── screenshots/
└── README.md
