# MULTI-CLOUD-ARCHITECTURE

COMPANY: CODTECH IT SOLUTIONS

NAME: NAGALAKSHMI L

INTERNID: CT12XJP

DOMAIN: CLOUD COMPUTING

DURATION: 12 WEEKS

MENTOR: NEELA SANTHOSH

# DESCRIPTION:

#  Multi-Cloud Architecture – Internship Task 3

##  Project Title:
**Multi-Cloud MERN Stack Application with AWS and Azure Integration**


## Task Objective

Design and demonstrate a **multi-cloud architecture** where services are distributed across **two cloud providers** (AWS and Azure). The goal is to showcase **interoperability** between platforms and ensure distributed, scalable, and resilient deployment.

---

##  Architecture Overview

###  AWS:
- **Frontend:** React App hosted on AWS S3 + CloudFront
- **Backend:** Node.js Express API deployed on EC2
- **Authentication:** AWS Cognito

### Azure:
- **Database:** Azure Cosmos DB (MongoDB API)
- **Optional Service:** Azure Functions for auxiliary processing (e.g., email or analytics)

---

##  Architecture Diagram

![Multi-Cloud Architecture Diagram](https://via.placeholder.com/800x400?text=Add+Your+Architecture+Diagram+Here)

---

## ⚙️ Setup & Configuration

###  AWS Components

1. **Frontend (React)**
   - Build React app: `npm run build`
   - Upload to AWS S3
   - Distribute via CloudFront

2. **Backend (Node.js)**
   - Deploy on EC2 instance
   - Configure security groups (open port 5000 or 3000)
   - Connect to Azure Cosmos DB via environment variables

###  Azure Components

1. **Azure Cosmos DB (MongoDB API)**
   - Create Cosmos DB instance
   - Enable MongoDB API compatibility
   - Update `.env` in backend:
     ```
     MONGO_URI="mongodb://<username>:<password>@<cosmos-db-uri>:10255/?ssl=true&replicaSet=globaldb"
     ```

2. **Optional: Azure Function**
   - Use for analytics, notifications, or webhook integrations
   - Accessible via REST API from the AWS backend

---

##  Interoperability Demonstration

###  Use Case Demonstrated:
- Frontend hosted on AWS → calls Node.js API on AWS → connects to **Cosmos DB on Azure**
- Optionally: Node.js API invokes **Azure Function** to send a notification or log data

### OUTPUT

![Image](https://github.com/user-attachments/assets/014e40f6-8683-4fe2-804b-ec4d8c6ad175)
![Image](https://github.com/user-attachments/assets/6218c093-ffad-4743-a292-a48b3146b37c)
![Image](https://github.com/user-attachments/assets/4348a7c1-a967-4eeb-a658-74aced04b0f1)
![Image](https://github.com/user-attachments/assets/ea2c4c48-520b-42cf-bb67-a23a1e4c9659)

