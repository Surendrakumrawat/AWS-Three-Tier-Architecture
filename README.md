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