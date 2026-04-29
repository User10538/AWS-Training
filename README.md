Overview

I designed and built a secure, cloud-native contact system using AWS serverless services. The goal was to create a scalable and production-ready solution that not only handles user submissions but also enforces strong security controls across multiple layers.

Problem

The initial contact form API was publicly accessible, meaning anyone could send requests. This created risks around spam, abuse, and unnecessary cost, and lacked visibility and persistence for submitted messages.

Solution

I implemented a secure, serverless architecture using Amazon Cognito, Amazon API Gateway, and AWS Lambda to enforce authentication and process requests.

User authentication is handled via Cognito’s hosted login, issuing JWT tokens that are validated by API Gateway before any request reaches the backend. The Lambda function processes validated requests, stores submissions in Amazon DynamoDB, and sends email notifications using Amazon SES.

To further strengthen security, I implemented geographic access control using AWS WAF, restricting access to Australian traffic only. IAM roles were configured with least-privilege permissions to tightly control service interactions, and logging was enabled through Amazon CloudWatch for debugging and monitoring.

Architecture
User → CloudFront → AWS WAF → Cognito → API Gateway → Lambda → DynamoDB + SES
Key Features
🔐 JWT-based authentication using Cognito
🛡️ API protection with API Gateway authorizer
🌍 Geo-restriction via AWS WAF (Australia-only access)
⚙️ Serverless backend with Lambda (Python)
🗄️ Persistent storage with DynamoDB
📬 Email notifications using SES
📊 Logging and debugging with CloudWatch
🔑 IAM least-privilege access control
Challenges & What I Learned

This project involved debugging across multiple AWS services, including handling CORS issues, resolving Lambda runtime errors, configuring IAM permissions, and understanding OAuth flows (authorization code vs implicit grant). Implementing JWT authentication and integrating it with API Gateway required careful configuration, particularly around token handling and request validation.

I also gained hands-on experience designing secure architectures, applying least-privilege access, and layering security controls using both identity-based and network-level protections.

Result

The system evolved from a public API into a secure, production-style backend where only authenticated users can submit requests. Messages are reliably stored and processed, and unauthorized or out-of-region traffic is blocked at the edge. The final architecture is scalable, maintainable, and aligned with AWS best practices for security and serverless design.

Tech Stack

☁️ AWS · 🔐 Cognito · 🧾 API Gateway · ⚙️ Lambda · 🗄️ DynamoDB · 📬 SES · 🛡️ WAF · 🌐 CloudFront · 📦 S3 · 📊 CloudWatch · 🔑 IAM
