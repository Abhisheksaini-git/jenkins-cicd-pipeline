# 📌 Project Overview

This project demonstrates an **Enterprise End-to-End CI/CD Pipeline** for deploying a Java Spring Boot application using modern DevOps tools.

The pipeline automatically builds, tests, scans, containerizes, publishes Docker images, and deploys applications to Kubernetes whenever new code is pushed to GitHub.

This project follows industry-standard DevOps practices and simulates a production-ready software delivery workflow.

# 🏗️ Architecture

                   Developer
                       │
                       ▼
              GitHub Repository
                       │
                       ▼
               GitHub Webhook
                       │
                       ▼
              Jenkins Pipeline
                       │
        ┌──────────────┼──────────────┐
        ▼              ▼              ▼
   Source Checkout   Maven Build   Unit Testing
                       │
                       ▼
              Trivy File System Scan
                       │
                       ▼
                 Docker Build
                       │
                       ▼
               Trivy Image Scan
                       │
                       ▼
                Push to Docker Hub
                       │
                       ▼
             Kubernetes Deployment
                       │
                       ▼
             Kubernetes Cluster
                       │
                       ▼
             Application Running

- Enterprise CI/CD Pipeline using Jenkins, Docker, Docker Hub, Kubernetes, Trivy and GitHub Actions for automated deployment.
