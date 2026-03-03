#  aws-cloud-infrastructure
# Enterprise-grade AWS infrastructure automation with Terraform - demonstrating cloud architecture patterns, resource provisioning, and IaC best practices.

# Highly Available Web Application Infrastructure (Terraform)

## Project Overview

This project provisions a highly available AWS networking foundation using Terraform as Infrastructure as Code (IaC).

It represents Phase 1 of a production-style, multi–Availability Zone web architecture designed following AWS best practices for scalability, fault tolerance, and network segmentation.

The objective of this phase is to establish a secure and extensible networking layer that will support application, load balancing, and database tiers in subsequent phases.

Architecture – Phase 1: Networking Foundation

This phase implements the core networking components required for a resilient cloud environment.

Region

us-east-1 (N. Virginia)

Resources Provisioned
1. Custom Virtual Private Cloud (VPC)

CIDR Block: 10.0.0.0/16

Provides logical isolation of cloud resources

Enables future subnet segmentation for multi-tier architecture

2. Public Subnets (Multi-AZ)

Two public subnets deployed across two Availability Zones

Designed to host internet-facing resources such as:

Application Load Balancers

Bastion Hosts (if required)

Public-facing services

3. Internet Gateway (IGW)

Attached to the VPC

Enables communication between VPC resources and the internet

4. Public Route Table

Associated with both public subnets

Includes route:

0.0.0.0/0 → Internet Gateway

5. Subnet Associations

Explicit subnet-to-route table associations

Ensures deterministic routing behavior

Aligns with infrastructure-as-code best practices

---

## The Architecture (Phase 1 – Networking Layer)
![Architecture Diagram](images/the-architecture.png)


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

    ---

##  AWS SimuLearn Lab Screenshots
File Systems in the Cloud

Description:
Implemented Amazon Web Services EFS to provide a fully managed, scalable file system accessible across multiple instances and availability zones, enabling shared storage for cloud applications.

![Computing Solutions](images/file-systems-in-cloud.png)

Amazon Bedrock Playground

Description:
Explored generative AI capabilities using Amazon Bedrock Playground to experiment with foundation models and AI-powered application features in a managed cloud environment.

Highly Available Web Applications

Description:
Designed a highly available architecture using multiple availability zones and an Application Load Balancer with health checks to distribute traffic and ensure application resilience.

![Computing Solutions](images/highly-available-web-applications.png)

Auto-Healing and Scaling Applications

Description:
Implemented auto-scaling and health-based instance recovery to enable self-healing applications that automatically replace unhealthy instances and scale based on demand.

![Computing Solutions](images/autohealing-and-scaling-applications.png)

Core Security Concepts (IAM Least Privilege)

Description:
Configured IAM groups and policies following least-privilege principles to restrict resource access and enhance cloud security.

![Computing Solutions](images/core-security-concepts.png)

First NoSQL Database (DynamoDB)

Description:
Modeled a serverless NoSQL database using DynamoDB to store and process user behavior data, enabling scalable data storage for analytics and application insights.

![Computing Solutions](images/first-nosql-database.png)

Databases in Practice (Amazon RDS Multi-AZ)

Description:
Migrated to Amazon RDS with multi-AZ deployment and read replicas to automate database management, improve availability, and enhance read performance.

![Computing Solutions](images/databases-in-practice.png)

Cloud Economics

Description:
Analyzed cloud cost structures and optimization strategies to maximize efficiency while leveraging scalable pay-as-you-go infrastructure.

### Connecting VPCs (VPC Peering)

Description:
Configured VPC peering to enable secure communication between networks, allowing resources in separate VPCs to interact while maintaining network isolation.

![Computing Solutions](images/connecting-vpcs.png)

Networking Concepts (VPC Configuration)

Description:
Set up VPC networking components including route tables, internet gateway, and security groups to establish secure and controlled internet connectivity.

Computing Solutions (EC2 Scaling)

Description:
Scaled EC2 instance capacity by upgrading instance type to improve application performance and support increased workload demands.

### Computing Solutions

Scaled the EC2 instance vertically by upgrading to a larger instance type to improve application performance and handle increased workload demand.


![Computing Solutions](images/aws-computing-solutions.png)