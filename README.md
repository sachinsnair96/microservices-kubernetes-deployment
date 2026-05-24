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
- User Service
- Product Service
- Order Service
- Gateway Service

## Services
- ClusterIP Services
- Kubernetes DNS-based communication
- Pod-to-pod networking

## Ingress
Configured path-based ingress routing for all services.

---

# Validation Performed

- Verified Minikube cluster
- Verified running pods
- Verified services
- Tested inter-service communication
- Verified ingress controller
- Tested external service access

---

# Kubernetes Screenshot Test

## Docker Running

![Docker](./screenshots/01_docker_running.png)

---

## Minikube Start

![Minikube](./screenshots/02_minikube_start.png)

---

## Nodes

![Nodes](./screenshots/03_kubectl_nodes.png)
