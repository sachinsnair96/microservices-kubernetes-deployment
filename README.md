# Microservices Kubernetes Deployment using Minikube

## Objective

The objective of this project is to deploy and validate a microservices-based application using Kubernetes and Minikube. This project demonstrates Kubernetes concepts such as:

- Deployments
- Services
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
- macOS Terminal

---

# Application Components

| Service Name | Description | Port |
|---|---|---|
| User Service | Handles user-related operations | 3000 |
| Product Service | Handles product-related operations | 3001 |
| Order Service | Handles order-related operations | 3002 |
| Gateway Service | API gateway and routing service | 3003 |

---

# Kubernetes Resources Implemented

## Deployments

Implemented Kubernetes deployments for:

- User Service
- Product Service
- Order Service
- Gateway Service

Each deployment includes:

- Labels and selectors
- Resource requests and limits
- Readiness probes
- Liveness probes

---

## Services

Implemented Kubernetes ClusterIP services for:

- User Service
- Product Service
- Order Service
- Gateway Service

These services enable:

- Internal cluster communication
- Kubernetes DNS-based service discovery
- Pod-to-pod communication

---

## Ingress Configuration

Implemented Kubernetes Ingress with path-based routing.

| Path | Routed Service |
|---|---|
| /api/users | User Service |
| /api/products | Product Service |
| /api/orders | Order Service |
| / | Gateway Service |

Ingress controller was enabled using Minikube addons.

---

# Validation Performed

The following validations were successfully completed:

- Verified Minikube cluster status
- Verified Kubernetes nodes
- Verified running pods
- Verified Kubernetes services
- Tested inter-service communication
- Verified ingress controller
- Tested ingress routing
- Verified external service access

---

# Project Structure

```text
submission/
├── deployments/
│   ├── gateway-service.yaml
│   ├── order-service.yaml
│   ├── product-service.yaml
│   └── user-service.yaml
├── services/
│   ├── gateway-service.yaml
│   ├── order-service.yaml
│   ├── product-service.yaml
│   └── user-service.yaml
├── ingress/
│   └── ingress.yaml
├── screenshots/
│   ├── 01_docker_running.png
│   ├── 02_minikube_start.png
│   ├── 03_kubectl_nodes.png
│   ├── 04_pods_all_namespaces.png
│   ├── 05_project_structure.png
│   ├── 06_user_service_pods.png
│   ├── 07_services_list.png
│   ├── 08_product_service_pods.png
│   ├── 09_order_service_pods.png
│   ├── 10_gateway_service_pods.png
│   ├── 11_services_all.png
│   ├── 12_service_communication.png
│   ├── 13_ingress_controller.png
│   ├── 14_ingress_test.png
│   └── 15_final_service_test.png
└── README.md
