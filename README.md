# Kubernetes — Container Orchestration & Cloud-Native Deployment Portfolio
## Deployments, Services, Storage, Secrets & Ingress (Production-Oriented)

![Kubernetes](https://img.shields.io/badge/Kubernetes-Container%20Orchestration-blue)
![DevOps](https://img.shields.io/badge/DevOps-Cloud--Native%20Deployment-green)
![MLOps](https://img.shields.io/badge/MLOps-Production%20Infrastructure-orange)


---

**Author:** Tirumala Teja Yegineni  
 

---

## 📌 Overview

This repository demonstrates **core Kubernetes (K8s) concepts and hands-on configurations** required to deploy and manage **stateful and stateless applications** in a **cloud-native environment**.

The focus is on **real-world Kubernetes primitives**, not just theory:
- Deployments
- Persistent storage
- Secrets management
- Ingress configuration
- Service exposure
- MySQL stateful workload deployment

These skills are critical for **DevOps, Platform Engineering, MLOps, and ML deployment at scale**.

---

## 📂 Repository Structure

```
Kubernetes-main/
│
├── kubernetes_notes.docx          # Kubernetes theory, concepts & explanations
│
├── projects/
│   ├── mysql-deploy.yaml          # MySQL Deployment
│   ├── mysql-config.yaml          # ConfigMap for MySQL
│   ├── mysql-secret.yaml          # Secrets (credentials)
│   ├── mysql-pvc.yaml             # PersistentVolumeClaim
│   └── ingress-config.yaml        # Ingress resource
```

---

# 🧪 Kubernetes Concepts Covered 

---

## 1️⃣ Kubernetes Architecture (Theory)

**Document:** `kubernetes_notes.docx`

### Concepts Covered
- Cluster architecture (Master / Control Plane, Worker Nodes)
- Core components:
  - API Server
  - Scheduler
  - Controller Manager
  - etcd
- Pods, Nodes, and Namespaces


“Explain Kubernetes architecture.”

---

## 2️⃣ Deployments (Stateless & Stateful Workloads)

**File:** `projects/mysql-deploy.yaml`

### What It Does
- Defines a **Deployment** for MySQL
- Manages pod lifecycle:
  - Replicas
  - Rolling updates
  - Self-healing

### Concepts Demonstrated
- Pod templates
- Replica management
- Declarative deployment

---

## 3️⃣ Configuration Management with ConfigMaps

**File:** `projects/mysql-config.yaml`

### What It Does
- Externalizes application configuration
- Injects environment-specific settings into containers

### Concepts Demonstrated
- Separation of config from code
- Environment portability
- Twelve-Factor App principles

---

## 4️⃣ Secrets Management

**File:** `projects/mysql-secret.yaml`

### What It Does
- Stores sensitive information securely:
  - Database usernames
  - Passwords

### Concepts Demonstrated
- Base64-encoded secrets
- Secure injection into pods
- Avoiding hardcoded credentials


“How do you manage secrets in Kubernetes?”

---

## 5️⃣ Persistent Storage (Stateful Workloads)

**File:** `projects/mysql-pvc.yaml`

### What It Does
- Defines a **PersistentVolumeClaim (PVC)**
- Ensures data persistence across pod restarts

### Concepts Demonstrated
- Stateful application handling
- Storage abstraction in Kubernetes
- Decoupling storage from pods

---

## 6️⃣ Ingress & External Access

**File:** `projects/ingress-config.yaml`

### What It Does
- Manages external HTTP access to services
- Routes traffic based on rules

### Concepts Demonstrated
- Ingress controllers
- Traffic routing
- Exposing services securely


“How do you expose applications in Kubernetes?”

---

## 🧠 How This Fits Into My Portfolio

This repository complements my work in:
- Dockerized applications
- FastAPI ML microservices
- MLOps pipelines
- Cloud-native ML deployments
- CI/CD and DevOps automation

It shows I can:
- Deploy **production-ready services**
- Handle **stateful workloads**
- Manage **configuration, secrets, and storage**
- Operate systems in **Kubernetes environments**

---

## ⚙️ How to Apply the Configurations (Example)

```bash
kubectl apply -f projects/mysql-config.yaml
kubectl apply -f projects/mysql-secret.yaml
kubectl apply -f projects/mysql-pvc.yaml
kubectl apply -f projects/mysql-deploy.yaml
kubectl apply -f projects/ingress-config.yaml
```

Check resources:
```bash
kubectl get pods
kubectl get svc
kubectl get pvc
kubectl get ingress
```

---

## 🧾 Points 

- Deployed a **stateful MySQL application on Kubernetes** using **Deployments, PersistentVolumeClaims, ConfigMaps, and Secrets**.  
- Implemented **configuration and secret management** to decouple application settings and credentials from container images.  
- Configured **persistent storage** to ensure data durability across pod restarts and rescheduling.  
- Exposed services using **Ingress resources**, enabling controlled external access to applications.  
- Built strong foundations in **cloud-native deployment, container orchestration, and Kubernetes operations**.

---

## 🧠 I Points

- “I understand Kubernetes primitives beyond basic Pods.”
- “I can deploy stateful services with persistent storage.”
- “I know how to manage secrets, configs, and ingress in production.”

---

## 👤 Author

**Tirumala Teja Yegineni**  
GitHub: https://github.com/TIRUMALA9999
