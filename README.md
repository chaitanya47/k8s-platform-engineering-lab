# Kubernetes Platform Engineering Lab

## 🚀 Objective
Designed and implemented a production-style Kubernetes platform simulating an on-premises developer infrastructure. This project focuses on platform engineering concepts including container orchestration, CI/CD automation, centralized authentication, and observability.

---

## 🏗 Architecture

<img width="1536" height="1024" alt="Project - 1 Architecture" src="https://github.com/user-attachments/assets/c175e643-be88-4a7e-8b88-cc6a9c02faca" />


---

## ⚙️ Tech Stack

- Kubernetes (kubeadm-based cluster)
- Docker
- AWS EC2 (simulating on-prem infra)
- Python (FastAPI for services)
- Helm (deployment packaging)
- GitHub Actions (CI/CD)
- Prometheus & Grafana (observability)

---

## 🔧 Key Components

### 1. Kubernetes Cluster
- Multi-node cluster setup using kubeadm
- Control plane + worker node architecture
- RBAC and networking configured

### 2. Application Service
- FastAPI-based microservice
- Containerized using Docker
- Deployed via Kubernetes

### 3. Centralized Authentication Service
- JWT-based authentication
- Role-based access control (RBAC)
- Stateless token validation

### 4. CI/CD Pipeline
- Automated build and deployment using GitHub Actions
- Docker image creation and registry push
- Continuous deployment to Kubernetes

### 5. Observability Stack
- Prometheus for metrics collection
- Grafana for visualization dashboards
- Structured logging and monitoring

---

## 🔄 CI/CD Workflow

1. Developer pushes code to GitHub
2. GitHub Actions builds Docker image
3. Image is pushed to Docker registry
4. Deployment triggered in Kubernetes cluster

---

## 🔐 Authentication Flow

1. User requests token from Auth Service
2. JWT token issued with role-based claims
3. Token used to access protected APIs
4. Services validate token before processing request

---

## 📊 Observability

- Metrics scraped using Prometheus
- Dashboards created in Grafana
- Alerts configured for system health monitoring

---

## 🧪 Failure Scenarios Tested

- Pod crash and restart handling
- Node failure simulation
- Token expiration handling
- Deployment rollback scenarios

---

## 📈 Key Learnings

- Kubernetes internals and cluster setup
- CI/CD pipeline design for container workloads
- Secure service-to-service authentication
- Observability and debugging distributed systems

---

## 📌 Future Improvements

- Add Horizontal Pod Autoscaling
- Implement custom Kubernetes operator
- Introduce service mesh (Istio)

---

## 🧑‍💻 Author

Chaitanya Sai Tadi  
DevOps Engineer – Kubernetes Platform & Infrastructure
