# Student-Registration-App
# 2-Tier Web Application Deployment on AWS
This repository showcases a **hands-on project** where I deployed a 2-Tier Web Application on AWS, implementing both application and database layers with a secure, scalable architecture.
## Project Overview
The project demonstrates the deployment of a **Student Registration Web Application** with a clear separation between the **Application Layer** and **Database Layer** in AWS using a custom VPC.

## Architecture

### Tier 1 – Application Layer
- **EC2 instance** (Ubuntu)
- **Nginx Web Server**
- **PHP 8.3**
- **Student Registration Web Application** (HTML + PHP)
- Hosted in a **public subnet**
- Internet access via **Internet Gateway**

### Tier 2 – Database Layer
- **EC2 instance** running MariaDB (MySQL)
- Hosted in a **private subnet**
- Database access restricted using **Security Groups**
- Connected securely to the application layer using **private IPs**

---

## Networking & Security
- **Custom VPC** with Public & Private Subnets
- **Route Tables** configured for proper traffic flow
- **Internet Gateway** for public access
- **NAT Gateway** to allow private subnet outbound internet access
- **Security Groups** for SSH, HTTP, and MySQL (3306) access control

---

## Key Tasks Performed
- ✅ Created **VPC**, **subnets**, and **route tables**
- ✅ Configured **Internet & NAT Gateways**
- ✅ Installed and configured **Nginx**, **PHP**, **MariaDB**
- ✅ Connected PHP application to MySQL database
- ✅ Implemented **form submission and database storage**
- ✅ Verified connectivity and security between tiers

---

## Skills & Concepts Gained
- AWS Networking (VPC, Subnets, Gateways, Security Groups)  
- Linux Server Configuration (Ubuntu, Nginx, PHP, MariaDB)  
- Web–Database Integration (PHP + MySQL)  
- Secure Cloud Architecture Design  

---

## Tech Stack
- **AWS Services:** EC2, VPC, Subnets, Internet Gateway, NAT Gateway, Security Groups  
- **Web Server:** Nginx  
- **Programming Languages:** PHP 8.3, HTML  
- **Database:** MariaDB (MySQL)  
- **OS:** Ubuntu  

---

## How to Run
1. Launch EC2 instances in the configured subnets.
2. Install Nginx and PHP on the application layer EC2.
3. Install MariaDB on the database layer EC2.
4. Configure security groups for SSH, HTTP, and MySQL access.
5. Connect PHP application to the database using private IPs.
6. Open the application URL from the public subnet EC2.

---


