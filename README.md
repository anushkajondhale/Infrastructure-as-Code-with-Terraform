# Terraform AWS Infrastructure as Code (IaC) 🚀

This project provisions and manages AWS infrastructure using **Terraform**, following the Infrastructure-as-Code (IaC) approach.  
It sets up a complete environment with VPC, subnets, security groups, EC2 instances behind a Load Balancer, and remote state storage in S3.

---

## 📌 Objectives
- Automate AWS resource provisioning
- Store Terraform state remotely in S3 for team collaboration
- Demonstrate Infrastructure Versioning with Git

---

## 🛠 Tech Stack
- [Terraform](https://developer.hashicorp.com/terraform)
- [AWS](https://aws.amazon.com/)
- **S3** – Remote state storage
- **VPC** – Custom networking
- **EC2** – Compute instances
- **ALB** – Application Load Balancer

---

## 📂 Features
1. **VPC Creation** – with custom CIDR block  
2. **Public Subnets** – spread across multiple Availability Zones  
3. **Security Groups** – allow SSH and HTTP traffic  
4. **EC2 Instances** – provisioned in subnets with Nginx  
5. **Load Balancer (ALB)** – distributes HTTP traffic across EC2s  
6. **S3 Backend** – stores Terraform state remotely  
7. **Git Versioning** – track and manage changes  

---

## ⚙️ Implementation Steps
1. **Plan the architecture** – VPC, subnets, security groups, EC2, and ALB  
2. **Write Terraform configs** – `.tf` files for provider, variables, resources, and backend  
3. **Configure S3 Backend** – for remote state storage  
4. **Run Terraform commands** – init, plan, apply, destroy  
5. **Version control** – push configs to GitHub  

---

## 📋 Prerequisites
- AWS account with programmatic access  
- AWS CLI installed & configured (`aws configure`)  
- Terraform installed → [Download](https://developer.hashicorp.com/terraform/downloads)  
- Git installed  

---

## 🚀 Usage

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/abhi-gadge1773/-Terraform-AWS-Infrastructure-as-Code-Project.git
cd -Terraform-AWS-Infrastructure-as-Code-Project

2️⃣ Initialize Terraform
terraform init

3️⃣ Validate the Configuration
terraform validate

4️⃣ Preview Changes
terraform plan

5️⃣ Apply Infrastructure
terraform apply

6️⃣ Destroy Infrastructure (Optional)
terraform destroy

📁 Project Structure
.
├── provider.tf     # AWS provider configuration
├── backend.tf      # Remote state in S3
├── variables.tf    # Input variables
├── main.tf         # VPC, Subnets, EC2, ALB, Security Groups
├── outputs.tf      # Output values
└── README.md       # Documentation

📜 License

This project is for educational purposes only. Use at your own risk.

