# AWS VPC Networking Project

This project demonstrates the design and deployment of a secure and scalable **Virtual Private Cloud (VPC)** environment on AWS.  
It was implemented using an **AWS-provided lab environment** to ensure a cost-free setup, while following real-world cloud architecture principles.

---

## 📌 Table of Contents
- [Project Overview](#project-overview)
- [Architecture Diagram](#architecture-diagram)
- [VPC Design Components](#vpc-design-components)
- [Deployment Steps](#deployment-steps)
- [Security Configuration](#security-configuration)
- [Verification & Testing](#verification--testing)
- [Screenshots](#screenshots)
- [Conclusion](#conclusion)

---

## 🧭 Project Overview

This project focuses on building a **custom AWS network architecture** typically used in production deployments. It includes both public and private workloads, proper routing, secure access flow, and highly available subnets spread across multiple Availability Zones.

The goal is to demonstrate:
- Network segmentation  
- Secure resource placement  
- NAT-based outbound traffic for private workloads  
- Internet-accessible public hosts  
- Infrastructure documentation for a portfolio  

---

## 🖼 Architecture Diagram

Below is the architecture diagram created for this project:

![VPC Architecture Diagram](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/MyNetworkingVPC%20Architecture%20diagram.png?raw=true)

---

## 🧩 VPC Design Components

### **VPC**
- Custom VPC with a dedicated CIDR range

### **Subnets**
- **2 Public Subnets** (for internet-facing resources)
- **2 Private Subnets** (for internal workloads)
- Subnets distributed across multiple Availability Zones

### **Internet Gateway (IGW)**
- Allows outbound/inbound internet traffic for public resources

### **NAT Gateway**
- Allows private instances to reach the internet securely

### **Route Tables**
- **Public Route Table** → IGW  
- **Private Route Table** → NAT Gateway  

### **Security Groups**
- Public EC2 SG (allows HTTP + SSH from lab console environment)
- Private EC2 SG (allows internal subnet communication only)

### **EC2 Instances**
- **Public EC2 Instance** in Public Subnet  
- **Private EC2 Instance** in Private Subnet  

---

## 🚀 Deployment Steps

### **1. Create the VPC**
- Defined CIDR block  
- Enabled DNS hostname support  

### **2. Create Public & Private Subnets**
- 2 public subnets  
- 2 private subnets  
- Each mapped to an Availability Zone  

### **3. Attach an Internet Gateway**
- Created and attached to the VPC  
- Added route in Public Route Table  

### **4. Create NAT Gateway**
- Placed in a Public Subnet  
- Elastic IP assigned  
- Added route in Private Route Table  

### **5. Configure Route Tables**
- Public route → IGW  
- Private route → NATGW  
- Associated with relevant subnets  

### **6. Create Security Groups**
- Public SG → allows HTTP + SSH  
- Private SG → allows only internal traffic  

### **7. Launch EC2 Instances**
- Public EC2 → Public Subnet  
- Private EC2 → Private Subnet  
- Appropriate SGs attached  

---

## 🔐 Security Configuration

### Public Security Group
- **Inbound:**  
  - HTTP (80)  
  - SSH (22)  
- **Outbound:**  
  - Allow all (default)

### Private Security Group
- **Inbound:**  
  - Allow only traffic from Public SG  
- **Outbound:**  
  - Allow all (default)

---

## 🧪 Verification & Testing

- Verified public EC2 reaches the Internet  
- Verified private EC2 routes outbound traffic through NAT Gateway  
- Checked subnet and route table associations  
- Ensured isolation of private workload  
- Captured screenshots of each deployment step for documentation  

---

## 📸 Screenshots

Below are the screenshots of the deployment steps:
### 1. VPC Created
![VPC Created](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/vpc-created.png?raw=true)

### 2. Public Subnets
![Public Subnets](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Subnet-Public.png?raw=true)

### 3. Private Subnets
![Private Subnets](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Subnet-Private.png?raw=true)

### 4. InternetGW Created And Attached To A VPC
![Internet gw](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Internetgateway-attached-to-VPC.png?raw=true)

### 5. Public Route Table
![Public RT](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Routetable-created.png?raw=true)

### 6. Private Route Table
![Private RT](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Private-Route.png?raw=true)

### 7. Nat Gateway
![Nat GW](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Natgw.png?raw=true)

### 8. Private Route Table To Use Natgateway
![Private Route/Natgw](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Private-Route-To-Use-Natgw.png?raw=true)

### 9. Private EC2
![Private EC2](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Private-Ec2.png?raw=true)


### 10. Public EC2
![Public EC2](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Public-EC2.png?raw=true)

### 11. Private SG
![Private SG](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Private%20SG.png?raw=true)


### 12. Public SG
![Public SG](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Public%20SG.png?raw=true)




---

## ✅ Conclusion

This project demonstrates a production-style AWS networking foundation, showcasing skills in:

- VPC design and segmentation  
- Routing architecture  
- Secure internet access patterns (IGW & NAT)  
- Subnet planning across Availability Zones  
- EC2 deployment in isolated networks  
- Cloud documentation and diagramming  

This setup forms a strong foundation for future cloud projects such as load balancers, container platforms, or application deployments.

---
