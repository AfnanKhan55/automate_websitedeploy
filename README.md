# 🚀 Automated Kubernetes Website Deployment Using Kind

This project automates the deployment of a **static website** using **Docker**, **Kubernetes**, and **Kind (Kubernetes in Docker)**. It sets up a **local Kubernetes cluster**, builds a **Docker container for the website**, and deploys it inside the cluster.

## 📌 Features
✅ **Automated Deployment**: Deploys a website in a containerized environment.  
✅ **Uses Kind**: Creates a local Kubernetes cluster without cloud costs.  
✅ **Dockerized Website**: Uses **Nginx** to serve the static website.  
✅ **Port Forwarding**: Access the website locally on `http://localhost:8080`.  
✅ **Scalability**: Deploys with **2 replicas** for high availability.  

---

## ⚙️ Prerequisites
Before running the script, ensure you have the following installed:
- [Docker](https://www.docker.com/)
- [Kind](https://kind.sigs.k8s.io/)
- [Kubectl](https://kubernetes.io/docs/tasks/tools/)

---

## 🛠️ Installation & Setup
### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/your-repo/kind-website-deployment.git
cd kind-website-deployment
2️⃣ Run the Deployment Script

chmod +x deploy-website.sh
./deploy-website.sh
3️⃣ Access the Website
Once the deployment is complete, access your website at:
➡ http://localhost:8080

🛑 Cleanup (Delete All Resources)
To remove everything and free up space:

kind delete cluster --name demo-cluster
rm -rf website deployment.yaml service.yaml
📌 Notes
This script is designed for local Kubernetes testing and is not for production use.
Modify index.html to customize your website.
Increase replicas in deployment.yaml for better scalability.
📧 Support
For any issues, feel free to contact Afnan Khan or open an issue in the repository. 🚀
