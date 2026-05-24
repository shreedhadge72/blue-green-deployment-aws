
# 🚀 Blue-Green Deployment on AWS using Docker
## 📌 Project Overview
This project demonstrates a **Blue-Green Deployment strategy** using AWS EC2 instances and Docker containers. It ensures zero-downtime deployment by switching traffic between two identical environments (Blue and Green) using an AWS Application Load Balancer.
---
## 🏗️ Architecture Diagram
![Architecture](screenshots/blue-green-deployment-diagram.png)
---
## 🔄 Deployment Workflow
- Developer writes code locally
- Code is pushed to GitHub
- AWS EC2 instances are created (Blue & Green)
- Docker containers are deployed on both environments
- AWS Load Balancer routes traffic between environments
- Users access the application seamlessly
---
## ☁️ AWS Components Used
- EC2 Instances (Blue & Green)
- Application Load Balancer (ALB)
- Security Groups
- Ubuntu Server
---
## 🐳 Docker Setup
Each environment runs a Docker container hosting a simple web application.
Example commands used:
```bash
docker build -t blue-app .
docker run -d -p 8080:80 blue-app
```
---
## 📸 Screenshots
### 🔵 Blue Environment
![Blue](screenshots/local-blue.png)
### 🟢 Green Environment
![Green](screenshots/local-green.png)
### 🐳 Docker Containers Running
![Docker](screenshots/docker-containers-local.png)
### ☁️ AWS Load Balancer
![ALB](screenshots/aws-load-balancer.png)
### 🎯 Target Group Health
![Health](screenshots/target-group-health.png)
---
## 🔁 Load Balancer Output
### Blue Traffic
![Blue Output](screenshots/load-balancer-output-blue.png)
### Green Traffic
![Green Output](screenshots/load-balancer-output-green.png)
---
## 🎯 Key Features
- Zero downtime deployment
- Easy rollback (switch Blue/Green)
- Scalable architecture
- Real-world DevOps workflow
---
## 📌 Author
Shree Dhadge
---
## ⭐ Learning Outcome
- AWS EC2 setup
- Docker containerization
- Load balancing concepts
- Blue-Green deployment strategy
---

