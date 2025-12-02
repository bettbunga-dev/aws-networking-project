AWS VPC Networking Project
Overview

This project demonstrates how to design and implement a custom Virtual Private Cloud (VPC) in AWS.
It includes subnets, route tables, an Internet Gateway, a NAT Gateway, EC2 instances, and proper routing architecture.


All resources were deployed using an AWS-provided lab environment.

📐 VPC Architecture

VPC Configuration Includes:

Custom VPC

2 Public Subnets

2 Private Subnets

Internet Gateway

NAT Gateway

Route Tables (Public + Private)

EC2 Instances placed in the correct subnets


Architecture Diagram:
## VPC Architecture

Below is the architecture diagram for the VPC setup used in this project:

![VPC Architecture Diagram](https://github.com/bettbunga-dev/aws-networking-project/blob/main/project1-networking/screenshots/MyNetworkingVPC%20Architecture%20diagram.png?raw=true)


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



🎯 What I Learned

VPC design fundamentals

Public vs private subnet routing

How NAT and Internet Gateways work

EC2 network accessibility rules

AWS networking best practices



📎 LinkedIn Post

I also shared this project on LinkedIn as part of my cloud portfolio:
(You will paste your LinkedIn post link here once we create it.)
