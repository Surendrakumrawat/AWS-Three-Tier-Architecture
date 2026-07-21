# AWS Three-Tier Architecture

<p align="center">

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws)
![EC2](https://img.shields.io/badge/EC2-Application_Server-blue)
![RDS](https://img.shields.io/badge/RDS-MySQL-success)
![ALB](https://img.shields.io/badge/Application_Load_Balancer-red)
![VPC](https://img.shields.io/badge/VPC-Networking-blueviolet)
![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black?logo=github)

</p>

---

# 📌 Project Overview

This project demonstrates a **Highly Available AWS Three-Tier Architecture** built using Amazon Web Services (AWS).

The architecture separates the application into three independent layers:

- Web Tier
- Application Tier
- Database Tier

Each layer is deployed inside dedicated subnets to improve **Security, Scalability, High Availability, and Fault Tolerance**.

---

# 🏗 Architecture Diagram

<p align="center">

<img src="Architecture/architecture-diagram.png" width="900">

</p>

---

# 📖 Architecture Documentation

Detailed architecture explanation is available here:

📂 **Architecture/architecture.md**

---

# 🚀 AWS Services Used

| Service | Purpose |
|----------|----------|
| Amazon VPC | Network Isolation |
| Public Subnets | Load Balancer Layer |
| Private App Subnets | EC2 Application Servers |
| Private DB Subnets | Amazon RDS |
| Internet Gateway | Internet Access |
| NAT Gateway | Outbound Internet for Private Subnets |
| Route Tables | Traffic Routing |
| Security Groups | Firewall |
| Amazon EC2 | Application Server |
| Application Load Balancer | Traffic Distribution |
| Target Group | ALB Backend |
| Amazon RDS MySQL | Database |
| Git | Version Control |
| GitHub | Project Repository |

---

# ⭐ Project Features

- Highly Available Architecture
- Secure Network Design
- Public & Private Subnets
- Internet Gateway
- NAT Gateway
- Application Load Balancer
- Amazon EC2
- Amazon RDS MySQL
- Professional Documentation
- GitHub Ready Project

---


# 📂 Repository Structure

```text
AWS-Three-Tier-Architecture
│
├── Architecture
│   ├── architecture.md
│   └── architecture-diagram.png
│
├── Commands
│   └── commands.md
│
├── Website
│   └── index.html
│
├── Screenshots
│   ├── 01-production-vpc-created.png
│   ├── 02-public-web-subnet-az1-created.png
│   ├── 03-public-web-subnet-az2-created.png
│   ├── ...
│   └── 31-application-loaded-through-alb.png
│
└── README.md
```

---

# 📋 Prerequisites

Before starting this project, make sure you have:

- AWS Account
- Basic Linux Knowledge
- Basic Networking Knowledge
- Git Installed
- GitHub Account
- Visual Studio Code

---

# ⚙️ Implementation Steps

## Step 1 — Create Production VPC

- Create Production VPC
- CIDR Block: 10.0.0.0/16

---

## Step 2 — Create Public Subnets

- Public Web Subnet AZ1
- Public Web Subnet AZ2

---

## Step 3 — Create Private Application Subnets

- Private App Subnet AZ1
- Private App Subnet AZ2

---

## Step 4 — Create Private Database Subnets

- Private DB Subnet AZ1
- Private DB Subnet AZ2

---

## Step 5 — Configure Internet Gateway

- Create Internet Gateway
- Attach Internet Gateway to Production VPC

---

## Step 6 — Configure NAT Gateway

- Create NAT Gateway
- Associate Elastic IP
- Deploy inside Public Subnet

---

## Step 7 — Configure Route Tables

- Public Route Table
- Private Route Table
- Associate Public Subnets
- Associate Private Subnets

---

## Step 8 — Configure Security Groups

- Web ALB Security Group
- App Server Security Group
- Database Security Group

---

## Step 9 — Create Database Layer

- Create DB Subnet Group
- Launch Amazon RDS MySQL

---

## Step 10 — Launch Application Server

- Launch Amazon EC2
- Install Apache
- Deploy Sample Application

---

## Step 11 — Configure Target Group

- Create Target Group
- Register EC2 Instance

---

## Step 12 — Create Application Load Balancer

- Internet-facing ALB
- Listener HTTP:80
- Forward Requests to Target Group

---

## Step 13 — Verify Application

- Check Target Health
- Open ALB DNS
- Verify Application Response

---

# 🌐 Website Response

```
Hello from the Application Tier!

AWS Three-Tier Architecture Project
``


---

# 📸 Project Screenshots

## 1. Production VPC

![Production VPC](Screenshots/01-production-vpc-created.png)

---

## 2. Public & Private Subnets

![Public Web Subnet](Screenshots/02-public-web-subnet-az1-created.png)

![Private App Subnet](Screenshots/04-private-app-subnet-az1-created.png)

---

## 3. Internet Gateway

![Internet Gateway](Screenshots/08-production-igw-attached.png)

---

## 4. NAT Gateway

![NAT Gateway](Screenshots/09-production-nat-gateway-created.png)

---

## 5. Route Table Configuration

![Route Table](Screenshots/13-private-route-table-created.png)

---

## 6. Security Groups

![Security Groups](Screenshots/16-web-alb-security-group-created.png)

---

## 7. Amazon RDS

![Amazon RDS](Screenshots/20-rds-database-available.png)

---

## 8. EC2 Application Server

![EC2](Screenshots/23-app-server-running.png)

---

## 9. Target Group

![Target Group](Screenshots/25-target-group-created.png)

---

## 10. Application Load Balancer

![Application Load Balancer](Screenshots/29-alb-active.png)

---

## 11. Healthy Targets

![Healthy Targets](Screenshots/30-target-group-healthy.png)

---

## 12. Final Output

![Application](Screenshots/31-application-loaded-through-alb.png)

---


# 💻 Commands Used

See complete command reference here:

📂 **Commands/commands.md**

---

# 🎯 Skills Learned

- AWS Networking
- Amazon VPC
- Public & Private Subnets
- Internet Gateway
- NAT Gateway
- Route Tables
- Security Groups
- Amazon EC2
- Apache Web Server
- Application Load Balancer
- Target Groups
- Amazon RDS MySQL
- Git
- GitHub
- Linux Administration
- High Availability Architecture
- Three-Tier Deployment
- AWS Best Practices

---

# 🏆 Project Outcome

This project successfully demonstrates how to deploy a secure and highly available Three-Tier Architecture on AWS.

The application is deployed behind an **Application Load Balancer**, hosted on **Amazon EC2**, and designed to communicate with an **Amazon RDS MySQL** database inside private subnets. The network is secured using **VPC**, **Public & Private Subnets**, **Route Tables**, **Internet Gateway**, **NAT Gateway**, and **Security Groups**.

This project follows AWS architectural best practices for security, scalability, and high availability.

---

# 🚀 Future Improvements

This architecture can be further enhanced by adding:

- Auto Scaling Group (ASG)
- HTTPS using AWS Certificate Manager (ACM)
- Amazon Route 53
- AWS WAF
- Amazon CloudFront
- Amazon CloudWatch Monitoring
- AWS Systems Manager
- AWS Backup
- CI/CD using GitHub Actions or AWS CodePipeline

---

# 📚 References

- AWS Documentation
- Amazon EC2 Documentation
- Amazon VPC Documentation
- Amazon RDS Documentation
- Application Load Balancer Documentation

---

# 🧠 Skills Demonstrated

## AWS Services

- Amazon VPC
- Public & Private Subnets
- Internet Gateway
- NAT Gateway
- Route Tables
- Security Groups
- Amazon EC2
- Amazon RDS
- Application Load Balancer
- Target Groups

## Operating System

- Amazon Linux 2023

## Web Server

- Apache HTTP Server

## Networking

- CIDR
- Routing
- High Availability
- Network Segmentation

## Version Control

- Git
- GitHub

## Documentation

- Markdown
- GitHub Project Documentation
- Architecture Documentation

---

# 📄 License

This project is created for learning, practice, and portfolio purposes.

---

# 👨‍💻 Author

## Surendra Kumrawat

AWS Cloud | Git & GitHub | Linux | Networking | Cloud Projects

---

⭐ If you found this project useful, consider giving this repository a **Star**.

