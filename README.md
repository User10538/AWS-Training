AWS Cloud & Security Engineering Projects

Cloud-native AWS projects focused on secure infrastructure, serverless architecture, CI/CD automation, and cloud security engineering.

This repository contains hands-on projects built to strengthen practical experience across AWS services, secure backend development, infrastructure automation, and operational monitoring systems.

Core Focus Areas
Serverless Architecture
Secure API Design
AWS Cloud Security
IAM Least-Privilege Access Control
CI/CD Automation
Infrastructure as Code (Terraform)
Cloud Monitoring & Telemetry
Edge Security with CloudFront & AWS WAF
Featured Projects
Secure Serverless Backend API

Designed and secured a serverless backend API using Amazon Cognito and API Gateway JWT authorization to enforce authenticated access across protected routes. Implemented token validation prior to Lambda execution and integrated Amazon SES for secure server-side email processing.

Technologies:
Amazon Cognito • API Gateway • AWS Lambda • JWT • OAuth 2.0 • Amazon SES • CloudFront

AWS Serverless Security Monitoring Dashboard

Designed and deployed a serverless security monitoring platform on AWS using API Gateway, Lambda, and DynamoDB to collect and visualize security telemetry in real time. Implemented event-driven ingestion pipelines, IAM least-privilege access controls, and CloudFront-based HTTPS delivery.

Technologies:
AWS Lambda • API Gateway • DynamoDB • Amazon S3 • CloudFront • IAM • Cloudflare • Python • JavaScript

Secure AWS Static Website Architecture

Implemented a hardened static website architecture using private Amazon S3, CloudFront Origin Access Control (OAC), and AWS WAF. Applied edge-layer protections including rate limiting and managed rule sets to reduce origin exposure and mitigate common web threats.

Technologies:
AWS WAF • CloudFront • Amazon S3 • OAC • Terraform

AWS Static Website + CI/CD Pipeline

Designed and deployed a static web platform on AWS using S3 and CloudFront, with automated CI/CD workflows through GitHub Actions. Implemented HTTPS, custom domain integration via Cloudflare, and infrastructure automation using Terraform.

Technologies:
AWS • GitHub Actions • CloudFront • Cloudflare • Terraform

Serverless Contact Form API

Developed a secure serverless contact form platform using API Gateway, AWS Lambda, and Amazon SES for scalable email delivery. Implemented CORS handling, input validation, and CloudFront integration to support secure frontend-to-API communication.

Technologies:
AWS Lambda • API Gateway • Amazon SES • CloudFront • Python • Serverless Architecture

Technologies & Services
AWS Lambda
Amazon API Gateway
Amazon Cognito
Amazon DynamoDB
Amazon S3
Amazon CloudFront
AWS WAF
Amazon SES
IAM
Terraform
GitHub Actions
Python
JavaScript
Cloudflare
Engineering Principles

Projects in this repository emphasize:

Secure-by-default architecture
Least-privilege IAM design
Event-driven serverless systems
Infrastructure automation
Cloud-native scalability
Operational visibility and monitoring
Edge security and HTTPS enforcement
Repository Structure
/cloud-security-portfolio
│── README.md
│── frontend/
About

Cloud Engineer & Security-Focused Backend Developer building secure cloud-native systems using AWS serverless technologies, infrastructure automation, and cloud security best practices.
