# Dockerized Web Application with CI/CD Pipeline

## 📌 Project Overview
This project demonstrates a containerized web application deployed using Docker and Docker Compose, along with a CI/CD pipeline implemented using Jenkins.

## Live Access
- Frontend Application URL: http://3.110.219.188
- Backend API: http://3.110.219.188:5000

The objective of this assignment is to showcase DevOps skills including:
- Containerization
- Reverse proxy using Nginx
- CI/CD pipeline configuration
- Basic system design principles
- 
## 🏗️ System Architecture
The application consists of the following components:

1. **Frontend**
   - Runs as a Docker container
   - Serves the UI of the application

2. **Backend**
   - Runs as a Docker container
   - Handles API/business logic

3. **Database**
   - MySQL container
   - Persistent data using Docker volumes

4. **Nginx**
   - Acts as a reverse proxy
   - Routes traffic to frontend and backend services

All services communicate using a custom Docker network.

---

## 📂 Project Structure
---
## 🐳 Docker Compose
Docker Compose is used to manage multi-container setup including:
- Frontend
- Backend
- Database
- Nginx

Features:
- Custom bridge network
- Persistent volume for database
- Port mappings for external access
- Restart policy for high availability
---
## 🌐 Nginx Configuration
Nginx is configured as a reverse proxy to:
- Route `/` requests to frontend service
- Route `/api` requests to backend service

This improves scalability and separation of concerns.
---
## 🔁 CI/CD Pipeline (Jenkins)
The Jenkins pipeline performs the following steps:

1. Pulls source code from GitHub
2. Builds Docker images
3. Runs containers using Docker Compose
4. Ensures successful deployment

Pipeline is defined using a `Jenkinsfile`.
---
## 🚀 High Availability & Best Practices
- Containers ensure application isolation
- Restart policies enable fault tolerance
- Volumes provide data persistence
- Can be extended to Kubernetes for scalability
- Caching layers (Redis) can be added in future
---
## 📌 How to Run the Project
```bash
git clone <repository-url>
cd project-directory
docker-compose up -d

---

Author
Faiz Ansari
📧 Email: faizrabbani15373@gmail.com
📞 Phone: 9709153190
🔗 GitHub: https://github.com/faiz-ansari
