---

# SIT323/SIT737 – Cloud Native Application Development  
## 🧩 Task 6.2C – Interacting with Kubernetes

---

## 📘 Overview

This task builds on Task 6.1P by demonstrating how to interact with a Kubernetes cluster using the `kubectl` command-line tool. You'll verify the deployed application, forward local ports to access it, and optionally use the Kubernetes Dashboard for visualization.

---

## 🛠️ Required Tools

- [Git](https://git-scm.com/)  
- [Visual Studio Code](https://code.visualstudio.com/)  
- [Node.js](https://nodejs.org/en/download/)  
- Docker  
- Kubernetes (Minikube recommended)  
- Kubectl

---

## 🚀 Steps to Complete the Task

### ✅ 1. Verify Application Status

Use the following commands to check if your application is running:

```bash
kubectl get pods
kubectl get services
```

These will display all running pods and services in the cluster.

---

### 🔁 2. Forward Local Port to Kubernetes Service

To access the application via your browser, forward a local port to your Kubernetes service:

```bash
kubectl port-forward svc/calculator-service 3000:3000
```

> Replace `calculator-service` with your actual service name if it's different.

---

### 🌐 3. Open the App in Your Browser

Once port forwarding is active, open:

```
http://localhost:3000
```

You should now be able to interact with the deployed Node.js calculator application.

---

## 📊 Optional: Launch Kubernetes Dashboard

If you're using **Minikube**, you can also view your application visually via the Kubernetes Dashboard:

```bash
minikube dashboard
```

This opens a web UI where you can monitor your pods, deployments, and services.

---

## ✅ Task Summary

In this task, you have:

- Verified the running status of pods and services
- Forwarded local ports to access the deployed app
- Interacted with the app through a web browser
- explored the Kubernetes Dashboard

---
