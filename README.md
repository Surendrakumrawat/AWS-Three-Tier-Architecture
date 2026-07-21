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

## 1. Production VPC Created

![Production VPC](Screenshots/01-production-vpc-created.png)

---

## 2. Public Web Subnet AZ1

![Public Web Subnet AZ1](Screenshots/02-public-web-subnet-az1-created.png)

---

## 3. Public Web Subnet AZ2

![Public Web Subnet AZ2](Screenshots/03-public-web-subnet-az2-created.png)

---

## 4. Private App Subnet AZ1

![Private App Subnet AZ1](Screenshots/04-private-app-subnet-az1-created.png)

---

## 5. Private App Subnet AZ2

![Private App Subnet AZ2](Screenshots/05-private-app-subnet-az2-created.png)

---

## 6. Private DB Subnet AZ1

![Private DB Subnet AZ1](Screenshots/06-private-db-subnet-az1-created.png)

---

## 7. Private DB Subnet AZ2

![Private DB Subnet AZ2](Screenshots/07-private-db-subnet-az2-created.png)

---

## 8. Internet Gateway Attached

![Internet Gateway](Screenshots/08-production-igw-attached.png)

---

## 9. NAT Gateway Created

![NAT Gateway](Screenshots/09-production-nat-gateway-created.png)

---

## 10. Public Route Table

![Public Route Table](Screenshots/10-public-route-table-created.png)

---

## 11. Public Route Added

![Public Route](Screenshots/11-public-route-added.png)

---

## 12. Public Subnet Associated

![Public Subnet Association](Screenshots/12-public-subnet-associated.png)

---

## 13. Private Route Table

![Private Route Table](Screenshots/13-private-route-table-created.png)

---

## 14. Private Route Added

![Private Route](Screenshots/14-private-route-added.png)

---

## 15. Private Subnets Associated

![Private Subnets](Screenshots/15-private-subnets-associated.png)

---

## 16. Web ALB Security Group

![Web Security Group](Screenshots/16-web-alb-security-group-created.png)

---

## 17. Application Server Security Group

![Application Security Group](Screenshots/17-app-server-security-group-created.png)

---

## 18. Database Security Group

![Database Security Group](Screenshots/18-database-security-group-created.png)

---

## 19. DB Subnet Group

![DB Subnet Group](Screenshots/19-db-subnet-group-created.png)

---

## 20. Amazon RDS Available

![Amazon RDS](Screenshots/20-rds-database-available.png)

---

## 21. EC2 Launch Configuration

![EC2 Launch](Screenshots/21-app-server-launch-configuration.png)

---

## 22. User Data Configuration

![User Data](Screenshots/22-app-server-user-data.png)

---

## 23. EC2 Running

![EC2 Running](Screenshots/23-app-server-running.png)

---

## 24. Target Group Configuration

![Target Group](Screenshots/24-target-group-configuration.png)

---

## 25. Target Group Created

![Target Group Created](Screenshots/25-target-group-created.png)

---

## 26. ALB Basic Configuration

![ALB Configuration](Screenshots/26-alb-basic-configuration.png)

---

## 27. ALB Network Mapping

![ALB Network](Screenshots/27-alb-network-mapping.png)

---

## 28. ALB Listener & Routing

![ALB Listener](Screenshots/28-alb-listener-routing.png)

---

## 29. Application Load Balancer Active

![ALB Active](Screenshots/29-alb-active.png)

---

## 30. Target Group Healthy

![Target Healthy](Screenshots/30-target-group-healthy.png)

---

## 31. Application Successfully Running

![Application Running](Screenshots/31-application-loaded-through-alb.png)

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










# AWS Three-Tier Architecture

## Project Overview

This project demonstrates a highly available and secure Three-Tier Architecture on AWS using Amazon VPC, EC2, Application Load Balancer (ALB), NAT Gateway, Internet Gateway, Route Tables, Security Groups, and Amazon RDS MySQL.

The architecture follows AWS best practices by separating the Web, Application, and Database layers into different subnets to improve security, scalability, and availability.

---

## Architecture

See the complete architecture diagram below.

👉 **Architecture/architecture.md**

---

## AWS Services Used

- Amazon VPC
- Public & Private Subnets
- Internet Gateway
- NAT Gateway
- Route Tables
- Security Groups
- Amazon EC2
- Application Load Balancer
- Target Group
- Amazon RDS MySQL

---

## Project Architecture

```
User
   │
   ▼
Application Load Balancer
   │
   ▼
Application Server (EC2)
   │
   ▼
Amazon RDS (MySQL)
```

---

## Project Structure

```
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
│   ├── ...
│   └── 31-application-loaded-through-alb.png
│
└── README.md
```

---

## Implementation Steps

- Created Production VPC
- Created Public and Private Subnets
- Configured Internet Gateway
- Configured NAT Gateway
- Created Route Tables
- Configured Security Groups
- Created DB Subnet Group
- Launched Amazon RDS MySQL
- Launched EC2 Application Server
- Configured Apache Web Server
- Created Target Group
- Created Application Load Balancer
- Verified Target Health
- Tested Application through ALB

---

## Screenshots

The **Screenshots** folder contains the complete implementation from VPC creation to successful application deployment.

Total Screenshots: **31**

---

## Result

The application was successfully deployed using a secure AWS Three-Tier Architecture.

The Application Load Balancer successfully routed user requests to the EC2 Application Server, which communicated securely with Amazon RDS inside private subnets.

---

## Author

**Surendra Kumrawat**

AWS Cloud | GitHub Portfolio