🌐 AWS VPC Networking Project
📌 Overview

This project demonstrates the design and implementation of a custom AWS Virtual Private Cloud (VPC) following real-world cloud networking best practices.

Using an AWS-provided ALX Lab Environment, I deployed a full networking infrastructure that includes:

Custom VPC

Public & Private Subnets

Internet Gateway

NAT Gateway

Public & Private Route Tables

Security Groups

Public & Private EC2 Instances

End-to-end routing configuration

This project showcases my understanding of AWS networking, infrastructure design, and cloud architecture documentation.

🏗️ VPC Architecture
🔧 Components Deployed

Custom VPC (CIDR: 10.0.0.0/16)

2 Public Subnets (for ALB and Bastion/Public EC2)

2 Private Subnets (for backend servers)

Internet Gateway (for public internet access)

NAT Gateway (to allow private EC2 outbound access)

Public Route Table (routes internet traffic via IGW)

Private Route Table (routes outbound traffic via NAT Gateway)

Security Groups

Public EC2 SG (HTTP + SSH restricted)

Private EC2 SG (backend access only)

EC2 Instances

Public EC2 Instance

Private EC2 Instance

🖼️ Architecture Diagram

📸 Deployment Screenshots

Below are screenshots of the deployment steps captured in the AWS lab environment:



Included Screenshots:

VPC creation

Subnets creation (Public & Private)

Internet Gateway attachment

NAT Gateway creation

Route Table configuration

Public EC2 instance

Private EC2 instance

Security Group configuration

Final verification

🧠 Skills Demonstrated

Through this project, I demostrated:

How to design a secure multi-tier VPC

Best practices for routing and subnet isolation

How public and private subnets interact

How NAT Gateways enable secure outbound internet access

How Security Groups enforce traffic control

How to document cloud infrastructure professionally

🧪 Steps Performed in the Lab

Created a new VPC with a custom CIDR block

Created public and private subnets

Attached an Internet Gateway

Configured route tables

Set up a NAT Gateway for private subnets

Launched EC2 instances in public and private subnets

Verified connectivity


Documented and captured screenshots

📸 Screenshots

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

### 8. Private SG
![Private SG](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Private%20SG.png?raw=true)


### 7. Public SG
![Public SG](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/Public%20SG.png?raw=true)


