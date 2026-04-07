<!-- ======================= -->
<!-- 🔥 HERO SECTION -->
<!-- ======================= -->

<h1 align="center">🌩️ Nimbus Docker Project</h1>

<p align="center">
  <b>Containerization · Docker · Azure Container Registry (ACR)</b>
</p>

<p align="center">
  Production-style Docker project demonstrating how to build, run, and deploy containerized applications to the cloud
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Docker-Containerization-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Azure-ACR-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/DevOps-Workflow-orange?style=for-the-badge"/>
</p>

---

# 🚀 Project Overview

<p align="center">
<b>Docker + Azure ACR = Production-Ready Container Deployment</b>
</p>

This project demonstrates a **complete containerization workflow**:

- Build a Docker image  
- Run and test locally  
- Inspect using Docker Desktop  
- Push to Azure Container Registry (ACR)  

👉 Focus: **real-world DevOps container workflow (local → cloud)**

---

# 🧱 Core Skills Demonstrated

## 🐳 Docker Fundamentals
- Containers vs Virtual Machines  
- Images vs Containers  
- Layered filesystem  
- Docker CLI & Docker Desktop  

## 📦 Application Containerization
- Writing a production-ready Dockerfile  
- Using `.dockerignore`  
- Building images (`docker build`)  
- Running containers with port mapping  

## ☁️ Cloud Deployment (Azure ACR)
- Logging into ACR  
- Tagging images for registries  
- Pushing images to Azure  
- Viewing repositories in Azure Portal  
- Versioning (`:v1`, `:latest`)  

---

# 🧠 System Workflow


Application Code
↓
Dockerfile
↓
Docker Image
↓
Run Locally (Docker Desktop)
↓
Tag Image
↓
Push to Azure Container Registry (ACR)
↓
Cloud Deployment Ready


---

# 🧱 Build & Run (Local)

## Build the image

```bash
docker build -t nimbus-site:latest .
```

Run the container
docker run --rm -p 8080:80 nimbus-site:latest
📸 Local Deployment
Dockerfile
<p align="center"> <img src="images/dockerfile.png" width="80%"> </p>
.dockerignore
<p align="center"> <img src="images/dockerignore.png" width="80%"> </p>
Running Container (Docker Desktop)
<p align="center"> <img src="images/containers.png" width="80%"> </p>
Application Running (http://localhost:8080
)
<p align="center"> <img src="images/site.png" width="85%"> </p>
☁️ Azure Container Registry (ACR)
Commands Used
az acr login --name nimbusrgacr9rw9b

docker tag nimbus-site:latest nimbusrgacr9rw9b.azurecr.io/nimbus-site:v1

docker push nimbusrgacr9rw9b.azurecr.io/nimbus-site:v1
📸 Cloud Deployment
Local Images
<p align="center"> <img src="images/dockerimages.png" width="85%"> </p>
Tagging & Pushing
<p align="center"> <img src="images/taggedandpushed.png" width="85%"> </p>
Push Output
<p align="center"> <img src="images/pushed.png" width="85%"> </p>
Azure Resource Group
<p align="center"> <img src="images/nimbus-rg.png" width="85%"> </p>
ACR Repository View
<p align="center"> <img src="images/azure%20repositories.png" width="85%"> </p>
🧩 Docker Image Analysis
Image Layers (Docker Scout)
<p align="center"> <img src="images/layers.png" width="85%"> </p>
📁 Repository Structure
code/
└── nimbus-site/
    ├── assets/
    ├── app.js
    ├── index.html
    ├── styles.css
    ├── nginx.conf
    ├── Dockerfile
    ├── .dockerignore
    └── README.md

images/
├── dockerfile.png
├── dockerignore.png
├── containers.png
├── dockerimages.png
├── layers.png
├── nimbus-rg.png
├── pushed.png
├── site.png
├── taggedandpushed.png
└── azure repositories.png
🔗 View Application Code
<p align="center"> <a href="https://github.com/seyiabello/Docker---Containerization-for-DevOps-Engineers/tree/master/code/nimbus-site"> <img src="https://img.shields.io/badge/View%20Application%20Code-000000?style=for-the-badge&logo=github"> </a> </p>
🧠 Skills Demonstrated
Category	Skills
Docker	Dockerfile, layers, images, containers, .dockerignore, port mapping
DevOps	Containerization, reproducible builds, local → cloud workflow
Azure	ACR login, tagging, pushing, repository inspection
Tooling	Docker Desktop, CLI operations
🎯 Project Outcome

✔ Application successfully Dockerized
✔ Container runs locally using Docker Desktop
✔ Image tagged and pushed to Azure Container Registry
✔ Cloud-ready container image
✔ End-to-end DevOps workflow demonstrated

✨ Summary
<p align="center"> <b> A production-style project demonstrating the ability to containerize, deploy, and ship applications using Docker and Azure. </b> </p> ```
