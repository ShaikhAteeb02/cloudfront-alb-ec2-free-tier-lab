# AWS CloudFront with ALB and EC2 (Free Tier)

Deploy a scalable web architecture on AWS Free Tier using CloudFront CDN, Application Load Balancer (ALB), and backend EC2 instance running Apache web server.

---

## Features

- EC2 instance running Apache web server
- Application Load Balancer for distributing traffic
- CloudFront CDN for global content delivery and caching
- Security groups configured for secure inbound traffic
- Health checks for ALB target monitoring

---

## Architecture Overview

The setup provisions an EC2 instance inside a VPC with security groups allowing SSH and HTTP traffic. An Application Load Balancer distributes incoming traffic to EC2. CloudFront is configured as a CDN in front of the ALB improving performance and reducing latency. Health checks ensure availability and automatic failover.

- EC2 instance with Apache server
- ALB with target group including EC2 instance
- CloudFront distribution pointing to ALB DNS
- Secure and scalable Free Tier implementation

---

## Setup Instructions

1. **Launch EC2 Instance**
   - Configure instance with Amazon Linux or preferred AMI.
   - Set security groups for SSH and HTTP.
   - Install Apache web server.
2. **Create Security Groups**
   - ALB security group allowing HTTP from internet.
   - EC2 security group allowing SSH and HTTP from ALB.
3. **Configure Application Load Balancer**
   - Set up ALB with public subnets.
   - Define target group with EC2 instance.
   - Configure health checks on HTTP.
4. **Set up CloudFront Distribution**
   - Origin points to ALB DNS.
   - Enable caching and global delivery.
5. **Test Deployment**
   - Access CloudFront URL to verify website availability.

---

> Connect with me on GitHub and LinkedIn for any questions or collaborations.

<p align="center">
  <a href="https://github.com/ShaikhAteeb02">
    <img src="https://img.shields.io/badge/GitHub-Profile-informational?style=for-the-badge&logo=github&logoColor=white&color=181717" alt="GitHub Profile" />
  </a>
  <a href="https://www.linkedin.com/in/ateeb-ahmed-shaikh-932234192/">
    <img src="https://img.shields.io/badge/LinkedIn-Profile-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Profile" />
  </a>
</p>
