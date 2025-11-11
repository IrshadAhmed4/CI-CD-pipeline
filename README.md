"Frontend CI/CD Pipeline (Docker + GitHub Actions)"

This project demonstrates a simple **CI/CD pipeline** using **GitHub Actions** and **Docker** to build and deploy a static website (served via NGINX).  
It automatically builds a Docker image from the `index.html` file in this repository and pushes it to **Docker Hub**.

---

## 🧩 Project Overview

- **Frontend Type:** Static website (HTML)
- **Web Server:** NGINX
- **Container Registry:** Docker Hub  
- **CI/CD Platform:** GitHub Actions
- **Repository Owner:** [irshadahmed04](https://hub.docker.com/u/irshadahmed04)

---

## ⚙️ How the Pipeline Works

### 1. **GitHub Actions Workflow**
Located in `.github/workflows/docker-build-push.yml`

Every time you push to the `main` branch, the workflow:

1. Checks out the repository  
2. Dynamically creates a Dockerfile using `index.html`  
3. Builds the Docker image  
4. Logs in to Docker Hub  
5. Pushes the image as:irshadahmed04/frontend:v12
6. This serves your static HTML file via NGINX inside a container.
7. Build and Push Automation
8. Required Repository Secrets
9. Deployment (EC2 / Kubernetes)
---

