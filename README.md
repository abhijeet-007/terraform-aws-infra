🚀 Terraform AWS Infrastructure Project
📌 Overview

This project provisions AWS infrastructure using Terraform with a modular and production-ready structure.

🧱 Architecture
VPC
EC2 Instance
S3 Bucket
Remote Backend (S3 + DynamoDB)

📂 Project Structure
modules/ → reusable infrastructure
env/ → environment-specific configs (dev, prod)
backend-setup/ → state management setup

🔐 Backend Setup
Run first:
cd backend-setup
terraform init
terraform apply

🚀 Deploy Dev Environment
cd env/dev
terraform init
terraform apply -var-file="dev.tfvars"

🧹 Destroy Infrastructure
terraform destroy

🔒 Best Practices Used
Remote backend (S3 + DynamoDB)
State locking
Modular architecture
Environment separation
Sensitive files ignored

🧠 Key Concepts Covered
Terraform Modules
Remote Backend
State Management
terraform import
terraform destroy
Multi-environment setup