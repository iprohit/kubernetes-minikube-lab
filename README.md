# kubernetes-minikube-lab
# 🚀 Kubernetes Minikube Lab

This project demonstrates how to deploy and manage a simple NGINX application on a **local Kubernetes cluster** using **Minikube**. It’s a great hands-on exercise to understand Kubernetes fundamentals like deployments, services, scaling, and using `kubectl`.

---

## 🛠️ Tools & Technologies Used

- **Minikube** – For running Kubernetes locally
- **kubectl** – CLI tool to interact with Kubernetes
- **Docker** – Containerization engine
- **YAML** – For Kubernetes configuration files

---

## 🎯 Project Objective

- Install and run a Kubernetes cluster using Minikube
- Deploy an NGINX application
- Expose it using a Kubernetes service
- Scale the deployment
- Inspect pods, services, and logs

---

## 📁 Project Structure

├── deployment.yaml # Deployment configuration for NGINX 
├── service.yaml # Service to expose the NGINX app 
├── screenshots/ # Folder containing verification screenshots 
# Project documentation


---

## ⚙️ Setup Instructions

### 1. Start Minikube

Start your local Kubernetes cluster:

```bash
minikube start

Deploy the Application
Apply the deployment config:
kubectl apply -f deployment.yaml

Expose the Deployment
Apply the service config:
kubectl apply -f service.yaml

Verify Deployment
Check the pods:
kubectl get pods

Check the services:
kubectl get services

5. Scale the Deployment
Scale the app to 5 replicas:

kubectl scale deployment nginx-deployment --replicas=5

6. Describe Pod for Logs
View detailed information and logs:
kubectl describe pod nginx-deployment-96b9d695-2444
Replace nginx-deployment-96b9d695-2444 with an actual pod name from kubectl get pods.

7. Access the Application
Use Minikube to open the service in your browser:
minikube service nginx-service
