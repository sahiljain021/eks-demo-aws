# 🚀 Containerized Flask App on AWS EKS

## 🌐 Live Demo
App was live at: http://a460cda085a7941d0b7e476fee056eac-1318786718.ap-south-1.elb.amazonaws.com
*(Cluster destroyed after project completion to avoid charges)*

## 🏗️ Architecture
Docker → ECR → EKS (Kubernetes) → LoadBalancer → User

## 🛠️ Tech Stack
- 🐍 Python Flask
- 🐳 Docker
- 📦 AWS ECR (Container Registry)
- ☸️ AWS EKS (Kubernetes)
- ⚙️ kubectl
- 🔧 eksctl
- 📈 HPA (Horizontal Pod Autoscaler)

## ✨ Features
- 🐳 Containerized Flask app using Docker
- 📦 Pushed image to AWS ECR
- ☸️ Deployed on EKS with 1 node (t3.small)
- 🌐 LoadBalancer service for public access
- 📈 HPA configured to auto-scale 1-3 pods at 60% CPU
- ❤️ Health check endpoint at /health

## 📸 Screenshots
### 🐳 Docker Build
![Docker Build](screenshots/docker_build.jpg)

### 📦 Docker Push to ECR
![Docker Push](screenshots/docker_push.jpg)

### 🖼️ Docker Images
![Docker Images](screenshots/docker_images.jpg)

### 📦 ECR Repository
![ECR](screenshots/ecr.jpg)

### ☸️ EKS Cluster
![EKS](screenshots/eks.jpg)

### 🌐 App Live on Kubernetes
![Live](screenshots/Hello_from_Kubernetes_.jpg)

### 🖥️ kubectl get nodes
![Nodes](screenshots/kubectl_get_nodes.jpg)

### 🐳 kubectl get pods
![Pods](screenshots/kubectl_get_pods.jpg)

### 📈 kubectl get hpa
![HPA](screenshots/kubectl_get_hpa.jpg)

### 🌐 kubectl get service
![Service](screenshots/kubectl_get_service_eks-demo-service.jpg)

## 💰 Cost
Cluster destroyed immediately after testing.
Total cost: ~$2-3 for a few hours of EKS usage.

## 📁 Files
- 📄 `app.py` — Flask application
- 🐳 `Dockerfile` — Container definition
- 📦 `requirements.txt` — Python dependencies
- ⚙️ `deployment.yaml` — Kubernetes deployment manifest
- 🌐 `service.yaml` — Kubernetes LoadBalancer service
- 📈 `hpa.yaml` — Horizontal Pod Autoscaler config
