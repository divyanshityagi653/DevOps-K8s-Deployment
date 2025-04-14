# 🚀 Task 5: Kubernetes NGINX Deployment using Minikube

This project demonstrates how to deploy a simple NGINX application using **Kubernetes** on a local **Minikube** cluster with Docker as the container runtime.

---

## 📁 Repository Structure

DevOps-K8s-Deployment/ 
├── deployment.yaml # Kubernetes Deployment for NGINX
├── service.yaml # NodePort service to expose NGINX 
├── Task-5-Kubernetes-NGINX.zip # ZIP with all screenshots 
├── screenshots/ # Folder with individual screenshots 
└── README.md # This documentation


---

## 🛠️ Technologies Used

| Tool       | Version      |
|------------|--------------|
| Minikube   | v1.35.0      |
| Kubernetes | v1.32.0      |
| Kubectl    | v1.30.0      |
| Docker     | 28.0.4       |
| OS         | Ubuntu 22.04 (WSL) |

---

## 📘 Task Summary

> 🧠 **Objective:** Deploy NGINX web server inside a Kubernetes cluster using Minikube.  
> 🔧 Tools: Docker, kubectl, Minikube.  
> 🖼️ Documentation includes YAML files and screenshots.  

---

## ⚙️ Steps Performed

### ✅ 1. Start Minikube Cluster

```bash
minikube start --driver=docker --memory=2200mb --cpus=2

 2. Create Deployment for NGINX
'''bash
kubectl create deployment my-nginx --image=nginx

3.Expose Deployment via NodePort
bash

kubectl expose deployment my-nginx --type=NodePort --port=80

4.Verify Access via curl

curl http://192.168.49.2:30283

You should see the default Welcome to nginx! HTML page in the response.

5.  Verify in Web Browser
Open a browser and navigate to:

cpp
http://192.168.49.2:30283

You should see the NGINX welcome page.

Screenshots
All screenshots are available inside the screenshots/ folder and in the ZIP archive.

Final Result
✔️ NGINX deployed successfully inside Minikube Kubernetes cluster

✔️ NodePort exposed and working

✔️ Verified via curl and browser

✔️ All steps documented with YAML and screenshots




















