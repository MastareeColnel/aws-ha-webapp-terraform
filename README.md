# Highly Available Web Application Infrastructure (Terraform)

## 📌 Project Overview

This project provisions a highly available AWS networking foundation using Terraform.  
It is the first phase of building a production-style, multi-AZ web architecture.

---

## 🏗 Architecture (Phase 1 – Networking Layer)

The following resources are provisioned:

- Custom VPC (10.0.0.0/16)
- Two Public Subnets (across two Availability Zones)
- Internet Gateway
- Public Route Table
- Route to Internet (0.0.0.0/0)
- Subnet-to-Route Table Associations

Region: **us-east-1 (N. Virginia)**

---

## 🛠 Tools Used

- Terraform >= 1.5
- AWS Provider ~> 5.0
- VS Code
- Git & GitHub

---

## 📂 Project Structure
