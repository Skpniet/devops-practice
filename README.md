# DevOps Practice Repository 🚀  
### AWS EKS Setup using Terraform

This repository contains **DevOps practice projects**, including **AWS EKS Cluster setup using Terraform**.

---

## 👤 Author  
**Shailesh Kumar**  
Cloud / DevOps / DevSecOps Engineer  

---

## 📌 Repository Overview  

This repo is created to practice:
- AWS Cloud Infrastructure  
- Kubernetes (EKS)  
- Terraform (Infrastructure as Code)  
- DevOps Automation  

---

## 📂 Folder Structure  

devops-practice/
│
├── eks setup/ # Terraform code to create EKS cluster
└── README.md # Project documentation


---

## 🏗 Project: AWS EKS Cluster Setup  

This project provisions:
- AWS EKS Cluster  
- Worker Node Group  
- VPC, Subnets, NAT Gateway  
- IAM Roles & Policies  
- Security Groups  
- Auto Scaling  

---

## 🛠 Prerequisites  

Install required tools:

### AWS CLI  
```bash
aws --version
aws configure

**##Terraform**
terraform -version
kubectl version --client
git --version

📥 Clone Repository
git clone https://github.com/Skpniet/devops-practice.git
cd devops-practice/eks\ setup

⚙️ Configure Terraform Variables

Edit terraform.tfvars or variables.tf

Example:
region       = "ap-south-1"
cluster_name = "shailesh-eks-cluster"
node_count   = 2
instance_type = "t3.medium"


🚀 Create AWS EKS Cluster
Step 1 — Initialize Terraform
terraform init

Step 2 — Validate
terraform validate

Step 3 — Plan
terraform plan

Step 4 — Apply (Create Cluster)
terraform apply
Type yes to continue.

🔗 Connect kubectl to EKS

aws eks update-kubeconfig --region ap-south-1 --name shailesh-eks-cluster

Verify:
kubectl get nodes

📦 Deploy Test App (Optional)
kubectl create deployment nginx --image=nginx
kubectl expose deployment nginx --type=LoadBalancer --port=80
kubectl get svc

🧹 Destroy Cluster (Optional)
terraform destroy

⚠️ Notes

AWS charges apply while cluster is running

Ensure IAM permissions allow EKS creation

Delete cluster after testing to avoid billing

📞 Contact

Shailesh Kumar
📧 Email: skpniet008@gmail.com

📱 Phone: 7042907701

⭐ Star this repo if you find it useful!

---

# ✅ **How To Upload README to GitHub (Simple)**  

1. Open repo  
2. Click **Add README**  
3. Paste content  
4. Click **Commit changes**

---
