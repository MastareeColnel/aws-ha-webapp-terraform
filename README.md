#  aws-cloud-infrastructure
# Enterprise-grade AWS infrastructure automation with Terraform - demonstrating cloud architecture patterns, resource provisioning, and IaC best practices.

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

##  AWS SimuLearn Lab Screenshots
File Systems in the Cloud

Description:
Implemented Amazon Web Services EFS to provide a fully managed, scalable file system accessible across multiple instances and availability zones, enabling shared storage for cloud applications.

Amazon Bedrock Playground

Description:
Explored generative AI capabilities using Amazon Bedrock Playground to experiment with foundation models and AI-powered application features in a managed cloud environment.

Highly Available Web Applications

Description:
Designed a highly available architecture using multiple availability zones and an Application Load Balancer with health checks to distribute traffic and ensure application resilience.

Auto-Healing and Scaling Applications

Description:
Implemented auto-scaling and health-based instance recovery to enable self-healing applications that automatically replace unhealthy instances and scale based on demand.

Core Security Concepts (IAM Least Privilege)

Description:
Configured IAM groups and policies following least-privilege principles to restrict resource access and enhance cloud security.

First NoSQL Database (DynamoDB)

Description:
Modeled a serverless NoSQL database using DynamoDB to store and process user behavior data, enabling scalable data storage for analytics and application insights.

Databases in Practice (Amazon RDS Multi-AZ)

Description:
Migrated to Amazon RDS with multi-AZ deployment and read replicas to automate database management, improve availability, and enhance read performance.

Cloud Economics

Description:
Analyzed cloud cost structures and optimization strategies to maximize efficiency while leveraging scalable pay-as-you-go infrastructure.

Connecting VPCs (VPC Peering)

Description:
Configured VPC peering to enable secure communication between networks, allowing resources in separate VPCs to interact while maintaining network isolation.

Networking Concepts (VPC Configuration)

Description:
Set up VPC networking components including route tables, internet gateway, and security groups to establish secure and controlled internet connectivity.

Computing Solutions (EC2 Scaling)

Description:
Scaled EC2 instance capacity by upgrading instance type to improve application performance and support increased workload demands.

### Computing Solutions

Scaled the EC2 instance vertically by upgrading to a larger instance type to improve application performance and handle increased workload demand.

![Computing Solutions Architecture](images/Computing-Solutions.png)