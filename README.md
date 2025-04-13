# Deploying a Secure EC2 Instance with S3 Access Using AWS CloudFormation

##  Project Overview
This project deploys a secure and basic AWS infrastructure using **AWS CloudFormation**, featuring an **EC2 instance** with access to an **S3 bucket** in a public subnet.

---

##  Architecture Components

- **VPC** → Custom Virtual Private Cloud (CIDR: `10.0.0.0/16`)
- **Subnet** → Public Subnet in `us-east-1a`
- **Internet Gateway** → Provides internet access
- **Route Table & Association** → Directs public traffic
- **Security Group** → Allows SSH from a specific IP and HTTPS from the internet
- **IAM Role & Instance Profile** → EC2 instance access to S3
- **EC2 Instance** → t2.micro Amazon Linux instance with S3 permissions
- **S3 Bucket** → Versioning enabled for data protection

---

## ✅ Key Features

-  **Secure Access** → SSH allowed only from your public IP  
-  **IAM Role Integration** → Securely grants S3 access to EC2  
-  **Versioned S3 Bucket** → Helps manage object changes  
-  **Fully Automated** → Provisioned with CloudFormation  

---

## 🚀 Deployment Guide

### Upload the Template to CloudFormation
You can deploy this stack using the AWS Management Console or AWS CLI:

**Console:**
1. Go to **CloudFormation > Stacks > Create Stack**
2. Upload the `template.yaml`
3. Click through the setup and launch the stack

