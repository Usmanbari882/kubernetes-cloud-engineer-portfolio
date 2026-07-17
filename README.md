# ☸️ Kubernetes Cloud Engineer Portfolio

## 📌 Project Overview

This repository represents my complete Kubernetes learning journey and hands-on practical implementation.

I have studied and implemented Kubernetes concepts from basic to advanced level, including Kubernetes architecture, workload management, networking, storage, security, monitoring, troubleshooting, and Azure Kubernetes Service (AKS).

The goal of this project is to demonstrate practical Kubernetes skills required for Cloud Engineer and Cloud Infrastructure roles.

---

# 🚀 Technologies & Tools Used

- Kubernetes
- kubectl
- Minikube
- Docker
- YAML Configuration Files
- Helm
- Azure Kubernetes Service (AKS)
- Azure Container Registry (ACR)

---

# ☸️ Kubernetes Topics Covered

## 1. Kubernetes Fundamentals

### Kubernetes Introduction
Understanding Kubernetes as a container orchestration platform used for deploying, managing, scaling, and maintaining containerized applications.

### Kubernetes Architecture

Covered Kubernetes internal components:

- Control Plane
- Worker Nodes
- API Server
- etcd
- Scheduler
- Controller Manager
- kubelet
- kube-proxy

Understanding how Kubernetes manages application lifecycle and cluster operations.

---

# 2. Kubernetes Installation & Setup

Implemented Kubernetes environment using:

- Minikube
- kubectl

Covered:

- Kubernetes Cluster Setup
- Cluster Management
- kubectl Commands
- Cluster Status Checking

---

# 3. Kubernetes Core Objects

## Pods

Learned:

- Pod Architecture
- Container Execution
- Pod Lifecycle
- Pod Management

## ReplicaSet

Implemented:

- Maintaining Pod Availability
- Managing Replica Count

## Deployment

Covered:

- Application Deployment
- Rolling Updates
- Rollback Strategy
- Scaling Applications

## StatefulSet

Implemented:

- Stateful Applications
- Stable Network Identity
- Persistent Storage Management

## DaemonSet

Learned:

- Running Pods on Every Node
- Monitoring and Logging Agent Deployment

## Jobs & CronJobs

Covered:

- One-time Tasks
- Scheduled Tasks Automation

---

# 4. Kubernetes Configuration Management

## ConfigMap

Implemented:

- Application Configuration Management
- Environment Variables

## Secret

Implemented:

- Sensitive Data Management
- Password and Credential Storage

---

# 5. Kubernetes Storage

Covered Kubernetes Storage Concepts:

## Volume

Understanding container data persistence.

## Persistent Volume (PV)

Learned:

- Storage Resource Management
- Cluster Storage Allocation

## Persistent Volume Claim (PVC)

Implemented:

- Requesting Storage for Applications
- Connecting Pods with Storage

## StorageClass

Covered:

- Dynamic Storage Provisioning
- Automated Storage Management

---

# 6. Kubernetes Networking

Implemented and studied:

## Kubernetes Services

Covered:

- ClusterIP
- NodePort
- LoadBalancer
- Headless Service

## Service Discovery

Learned:

- Kubernetes DNS
- Internal Communication Between Applications

## Network Policy

Covered:

- Pod Traffic Control
- Application Security

---

# 7. Application Availability

Studied Kubernetes Health Checks:

## Liveness Probe

Used for:

- Detecting Failed Containers
- Automatic Restart

## Readiness Probe

Used for:

- Checking Application Availability Before Traffic

## Startup Probe

Used for:

- Slow Starting Applications

---

# 8. Kubernetes Resource Management

Covered:

- CPU Requests
- Memory Requests
- CPU Limits
- Memory Limits
- ResourceQuota
- LimitRange

Understanding how Kubernetes manages application resources.

---

# 9. Kubernetes Security

Studied Kubernetes Security Concepts:

## Authentication

User Identity Verification.

## Authorization

Permission Management.

## RBAC

Implemented:

- Role
- ClusterRole
- RoleBinding
- ClusterRoleBinding

## Service Account

Understanding Application Identity Management.

---

# 10. Kubernetes Troubleshooting

Practiced troubleshooting using:

- kubectl logs
- kubectl describe
- kubectl events
- kubectl exec

Covered common issues:

- CrashLoopBackOff
- ImagePullBackOff
- Pending Pods
- Container Errors
- Networking Issues

---

# 11. Helm Package Manager

Studied:

- Helm Installation
- Helm Charts
- Values.yaml
- Releases
- Upgrade
- Rollback

Understanding Kubernetes Application Packaging and Deployment.

---

# 12. Kubernetes Monitoring

Covered:

- Metrics Server
- kubectl top commands
- Prometheus
- Grafana

Understanding:

- Resource Monitoring
- Application Performance Monitoring

---

# 13. Kubernetes Logging

Studied:

- Container Logs
- Centralized Logging Concepts
- Fluent Bit
- Elasticsearch
- Kibana

---

# 14. Kubernetes Scaling

Covered:

## Horizontal Pod Autoscaler (HPA)

Automatic Pod Scaling based on resource usage.

## Vertical Pod Autoscaler (VPA)

Automatic Resource Adjustment.

## Cluster Autoscaler

Automatic Node Scaling.

---

# 15. Backup & Disaster Recovery

Covered:

- Backup Concepts
- Restore Strategy
- etcd Backup
- Disaster Recovery
- RPO
- RTO

---

# 16. Azure Kubernetes Service (AKS)

Studied Microsoft Azure Managed Kubernetes Service.

Covered:

## AKS Architecture

Understanding:

- Azure Control Plane
- Node Pools
- Kubernetes Integration

## AKS Cluster Creation

Implemented:

- Azure CLI
- AKS Deployment
- Cluster Connection

## Azure Container Registry (ACR)

Covered:

- Container Image Storage
- Image Management

## AKS Networking

Studied:

- Azure Virtual Network Integration
- Pod Networking
- Service Networking

## AKS Security

Covered:

- Azure RBAC
- Identity Management
- Secure Cluster Access

## AKS Monitoring

Covered:

- Azure Monitor
- Log Analytics
- Prometheus
- Grafana

---

# 🛠 Practical Implementation

During this learning journey, I performed hands-on implementations including:

✅ Kubernetes Cluster Setup  
✅ Nginx Deployment  
✅ ConfigMap Implementation  
✅ Secret Management  
✅ Persistent Storage Setup  
✅ Stateful Applications  
✅ DaemonSet Deployment  
✅ Kubernetes Networking  
✅ Helm Setup  
✅ AKS Concepts  

---

# 🎯 Skills Demonstrated

- Kubernetes Administration
- Container Orchestration
- Cloud Native Application Management
- Infrastructure Deployment
- Storage Management
- Networking Configuration
- Security Implementation
- Monitoring & Troubleshooting

---

# 👨‍💻 Career Objective

This portfolio demonstrates my practical Kubernetes skills as part of my journey toward becoming a Cloud Engineer.

I am continuously improving my skills in Cloud Infrastructure, Kubernetes, Automation, and Cloud Native Technologies.# kubernetes-cloud-engineer-portfolio
Complete Kubernetes Cloud Engineer Portfolio with practical implementations, YAML configurations, networking, storage, security, monitoring and Azure AKS.
# Kubernetes Commands Reference Guide

یہ فائل Kubernetes Hands-on Practice میں استعمال ہونے والی اہم Commands کا Reference ہے۔

---

# 1. Kubernetes Cluster Check

## Cluster Status Check

```bash
kubectl cluster-info
```

Kubernetes Cluster کی Information دیکھنے کے لیے۔

---

## Nodes Check

```bash
kubectl get nodes
```

Cluster کے تمام Nodes دیکھنے کے لیے۔

---

## Node Details

```bash
kubectl describe node
```

Node کی مکمل Information دیکھنے کے لیے۔

---

# 2. Pod Management

## Pods دیکھنا

```bash
kubectl get pods
```

تمام Running Pods دیکھنے کے لیے۔

---

## Detailed Pod Information

```bash
kubectl describe pod <pod-name>
```

Pod کی مکمل Details اور Events دیکھنے کے لیے۔

---

## Pod کے اندر جانا

```bash
kubectl exec -it <pod-name> -- bash
```

Container کے اندر Shell Access لینے کے لیے۔

---

## Pod سے باہر آنا

```bash
exit
```

Container Shell سے واپس آنے کے لیے۔

---

## Pod Delete کرنا

```bash
kubectl delete pod <pod-name>
```

Pod delete کرنے کے لیے۔

---

# 3. YAML Files Deployment

## Resource Create کرنا

```bash
kubectl apply -f filename.yaml
```

YAML file سے Kubernetes Resource بنانے کے لیے۔

---

## Resource Delete کرنا

```bash
kubectl delete -f filename.yaml
```

YAML کے ذریعے بنایا گیا Resource ختم کرنے کے لیے۔

---

# 4. Deployment Management

## Deployment دیکھنا

```bash
kubectl get deployments
```

Deployments کی Information دیکھنے کے لیے۔

---

## Deployment Details

```bash
kubectl describe deployment <deployment-name>
```

Deployment کی مکمل Details کے لیے۔

---

## Deployment Scale کرنا

```bash
kubectl scale deployment <name> --replicas=3
```

Pods کی تعداد بڑھانے یا کم کرنے کے لیے۔

---

# 5. Service Management

## Services دیکھنا

```bash
kubectl get services
```

تمام Services دیکھنے کے لیے۔

---

## Service Details

```bash
kubectl describe service <service-name>
```

Service کی Details دیکھنے کے لیے۔

---

# 6. ConfigMap

## ConfigMap دیکھنا

```bash
kubectl get configmap
```

ConfigMaps دیکھنے کے لیے۔

---

## ConfigMap Details

```bash
kubectl describe configmap <name>
```

ConfigMap کی Information کے لیے۔

---

# 7. Secret Management

## Secrets دیکھنا

```bash
kubectl get secrets
```

Kubernetes Secrets دیکھنے کے لیے۔

---

## Secret Details

```bash
kubectl describe secret <name>
```

Secret Information دیکھنے کے لیے۔

---

# 8. Storage (PV & PVC)

## Persistent Volumes دیکھنا

```bash
kubectl get pv
```

Persistent Volumes دیکھنے کے لیے۔

---

## Persistent Volume Claims

```bash
kubectl get pvc
```

PVC Status دیکھنے کے لیے۔

---

## Volume Pod Test

```bash
kubectl exec -it nginx-volume-pod -- bash
```

Volume mounted Pod میں جانے کے لیے۔

---

## Website File Check

```bash
cd /usr/share/nginx/html
```

Nginx Website Directory میں جانے کے لیے۔

```bash
cat index.html
```

File Content دیکھنے کے لیے۔

---

# 9. StatefulSet

## StatefulSet دیکھنا

```bash
kubectl get statefulset
```

StatefulSets دیکھنے کے لیے۔

---

## Stateful Pod Delete Test

```bash
kubectl delete pod nginx-stateful-1
```

Pod delete کر کے دیکھنا کہ StatefulSet دوبارہ Pod بناتا ہے۔

---

# 10. DaemonSet

## DaemonSet دیکھنا

```bash
kubectl get daemonsets
```

DaemonSets دیکھنے کے لیے۔

---

## DaemonSet Deploy کرنا

```bash
kubectl apply -f nginx-daemonset.yaml
```

DaemonSet create کرنے کے لیے۔

---

# 11. Headless Service

## Headless Service Check

```bash
kubectl get services
```

Cluster IP None والی Service دیکھنے کے لیے۔

---

# 12. Logs اور Troubleshooting

## Pod Logs

```bash
kubectl logs <pod-name>
```

Container Logs دیکھنے کے لیے۔

---

## All Resources Check

```bash
kubectl get all
```

تمام Kubernetes Resources دیکھنے کے لیے۔

---

# 13. YAML File Management

## Files دیکھنا

```bash
ls
```

Directory کی Files دیکھنے کے لیے۔

---

## YAML File بنانا

```bash
nano filename.yaml
```

YAML Configuration لکھنے کے لیے۔

---

# 14. Helm

## Helm Version

```bash
helm version
```

Helm Installation Check کرنے کے لیے۔

---

## Helm Installation

```bash
sudo snap install helm --classic
```

Helm install کرنے کے لیے۔

---

# 15. Kubernetes Troubleshooting Commands

```bash
kubectl get events
```

Cluster Events دیکھنے کے لیے۔

```bash
kubectl describe pod <pod-name>
```

Pod Issues Troubleshoot کرنے کے لیے۔

---

# Kubernetes Project Summary

اس Project میں استعمال ہونے والی Technologies:

* Kubernetes Cluster
* Pods
* Deployments
* Services
* ConfigMaps
* Secrets
* Persistent Volume
* Persistent Volume Claim
* StatefulSet
* DaemonSet
* Headless Service
* Helm Basics

---

# Author

Muhammad Usman Bari

Cloud Engineer Portfolio Project

