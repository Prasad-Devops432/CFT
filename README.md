# 🛠️ AWS Auto Scaling with Private Subnets, Bastion Host & Load Balancer

This project demonstrates a scalable and secure AWS architecture featuring EC2 Auto Scaling Groups, private subnets, a bastion host for secure access, and a load balancer monitoring a Python-based web app. Built to simulate real-world performance scaling and secure network segmentation.

---

## 📐 Architecture Overview

![Architecture Diagram](diagrams/auto-scaling-architecture.png)

- **2x EC2 Instances** in a Private Subnet (auto-scaled)
- **1x Bastion Host** in Public Subnet for SSH into Private EC2s
- **1x NAT Gateway** for outbound access from private instances
- **Application Load Balancer** to distribute HTTP traffic
- Auto Scaling responds to **CPU utilization**
- One EC2 runs a Python app, the other starts empty (test auto scaling performance and distribution)

---

## ☁️ AWS Services Used

- **EC2**
- **Auto Scaling Group**
- **Launch Templates**
- **VPC with Public & Private Subnets**
- **Application Load Balancer**
- **NAT Gateway**
- **Security Groups & Route Tables**

---
