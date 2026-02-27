# Highly Available Web Application Infrastructure (Terraform)

## The Project Overview

This project provisions a highly available AWS networking foundation using Terraform.  
It is the first phase of building a production-style, multi-AZ web architecture.

---

## The Architecture (Phase 1 – Networking Layer)
![Architecture Diagram](images/architecture.png)

The following resources are provisioned:

- Custom VPC (10.0.0.0/16)
- Two Public Subnets (across two Availability Zones)
- Internet Gateway
- Public Route Table
- Route to Internet (0.0.0.0/0)
- Subnet-to-Route Table Associations

Region: **us-east-1 (N. Virginia)**

---

## All Tools Used

- Terraform >= 1.5
- AWS Provider ~> 5.0
- VS Code
- Git & GitHub

---

## 📂 Project Structure
## 📂 Project Structure

aws-ha-webapp-terraform/
├── provider.tf
├── main.tf
├── variables.tf
├── outputs.tf
├── user_data.sh
├── .gitignore
├── README.md
├── images/
│   └── architecture.png
└── screenshots/
    ├── vpc-created.png
    ├── ec2-running.png
    └── web-browser-test.png
