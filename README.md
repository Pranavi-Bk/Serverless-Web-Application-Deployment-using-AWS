# Serverless Web Application Deployment using AWS

## 📌 Project Overview
This project implements a **Serverless Web Application** for managing student information using **Amazon Web Services (AWS)**.  
The application allows users to **add and view student details** through a web interface without managing any physical or virtual servers.

It uses a **three-tier serverless architecture** with AWS services to ensure scalability, security, and cost efficiency.

---

## 🎯 Problem Statement
Traditional web applications depend on dedicated servers that require continuous maintenance, scaling, and monitoring, which increases cost and complexity.

This project addresses the problem by using a **serverless architecture**, allowing developers to focus on application logic while AWS handles infrastructure, scaling, and availability.

---

## ✅ Objectives
- Deploy a serverless web application using AWS
- Implement backend logic using AWS Lambda
- Store student data using DynamoDB
- Connect frontend and backend using API Gateway
- Host static frontend files using Amazon S3
- Secure and optimize delivery using CloudFront
- Demonstrate scalability and cost efficiency

---

## 🛠️ Technologies Used

| Technology | Purpose |
|----------|--------|
| Amazon S3 | Hosts static frontend files |
| AWS Lambda | Backend business logic |
| Amazon DynamoDB | NoSQL database for student data |
| Amazon API Gateway | REST API integration |
| Amazon CloudFront | Secure content delivery (CDN) |
| AWS IAM | Role-based access control |
| Python | Lambda function development |
| HTML, CSS, JavaScript | Frontend development |
| JSON | Data exchange format |

---

## 🏗️ System Architecture
The application follows a **three-tier serverless architecture**:

### 1️⃣ Presentation Tier
- Amazon S3 hosts the static website
- CloudFront provides HTTPS and global access

### 2️⃣ Application Tier
- API Gateway exposes REST APIs
- AWS Lambda executes backend logic
  - `insertStudentData` – inserts student records
  - `getStudent` – retrieves student records

### 3️⃣ Data Tier
- Amazon DynamoDB stores student information
- Table Name: `studentData`
- Partition Key: `Studentid`

---

## 🔄 Workflow
1. User accesses the web application via browser
2. Frontend sends requests to API Gateway
3. API Gateway triggers Lambda functions
4. Lambda reads/writes data in DynamoDB
5. Response is returned to frontend
6. CloudFront delivers content securely

---

## 📂 Project Structure
serverless-web-app-aws/
├── README.md
├── lambda/
│ ├── getStudent.py
│ └── insertStudentData.py
├── frontend/
│ ├── index.html
│ ├── scripts.js
│ └── styles.css
├── report/
│ └── Cloud_Architecture_Design_Report.pdf
└── screenshots/
---

## 🧪 Testing
- Lambda functions tested using AWS Lambda test events
- API methods tested in API Gateway
- Website tested using S3 and CloudFront URLs
- Data verified in DynamoDB table

---

## ⭐ Outcomes
- Successful insertion and retrieval of student data
- Fully serverless and scalable application
- No server maintenance required
- Secure and cost-effective deployment

---

## 👍 Advantages
- Automatic scalability
- Pay-as-you-use pricing model
- High availability and reliability
- Simplified deployment and maintenance

---

## ⚠️ Limitations
- Cold start latency in Lambda
- Limited execution time
- Debugging can be complex
- Requires internet access

---

## 🚀 Future Enhancements
- User authentication using Amazon Cognito
- Update and delete student records
- Monitoring using CloudWatch dashboards
- CI/CD using AWS Amplify

---

## 🏁 Conclusion
This project demonstrates the power of **serverless computing** by building a complete web application without managing servers.  
By leveraging AWS services like Lambda, DynamoDB, API Gateway, S3, and CloudFront, the system achieves scalability, security, and cost efficiency suitable for real-world applications.

---

## 👩‍💻 Authors
- **P. Prudvhi Sai**
- **B. K. Pranavi**
