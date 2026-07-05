# 📌 Project Overview

This project demonstrates an **Enterprise End-to-End CI/CD Pipeline** for deploying a Java Spring Boot application using modern DevOps tools.

The pipeline automatically builds, tests, scans, containerizes, publishes Docker images, and deploys applications to Kubernetes whenever new code is pushed to GitHub.

This project follows industry-standard DevOps practices and simulates a production-ready software delivery workflow.

# 🚀 CI/CD Pipeline Workflow

```text
+-----------+
| Developer |
+-----------+
      |
      v
+-------------------+
| GitHub Repository |
+-------------------+
      |
      v
+------------------+
| GitHub Webhook   |
+------------------+
      |
      v
+------------------+
| Jenkins Pipeline |
+------------------+
      |
      v
+------------------+
| Checkout Source  |
+------------------+
      |
      v
+------------------+
| Maven Build      |
+------------------+
      |
      v
+------------------+
| Unit Testing     |
+------------------+
      |
      v
+----------------------+
| Trivy FS Scan        |
+----------------------+
      |
      v
+----------------------+
| Docker Image Build   |
+----------------------+
      |
      v
+----------------------+
| Trivy Image Scan     |
+----------------------+
      |
      v
+----------------------+
| Push to Docker Hub   |
+----------------------+
      |
      v
+----------------------+
| Deploy to Kubernetes |
+----------------------+
      |
      v
+----------------------+
| Kubernetes Cluster   |
+----------------------+
      |
      v
+----------------------+
| Application Running  |
+----------------------+
```

- Enterprise CI/CD Pipeline using Jenkins, Docker, Docker Hub, Kubernetes, Trivy and GitHub Actions for automated deployment.
