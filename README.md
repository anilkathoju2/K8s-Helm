# 🚀 Full-Stack Microservices Project on Kubernetes using Helm

This project is a production-ready microservices architecture deployed on **Kubernetes** using **Helm & Helm Charts**.  
It includes:

- **Frontend:** Nginx  
- **Backend:** Node.js (multiple microservices if needed)  
- **Build Tool:** Maven  
- **Databases:** MongoDB, MySQL  
- **Caching / Messaging:** Redis, RabbitMQ  

Helm is used to package, configure, and deploy each service easily with reusable templates.

---

*** Docker Images ***

## 🎯 Kubernetes + Helm Deployment Flow

1. Build Docker images:
   ```bash
   docker build -t <registry>/frontend:latest frontend/
   docker build -t <registry>/backend:latest backend/
   docker push <registry>/frontend:latest
   docker push <registry>/backend:latest

*** few Helm commands ***
helm install chart_name .
helm list
helm upgrade chart_name
helm history chart_name
helm rollback chart_name oldverison
helm uninstall chart_name




