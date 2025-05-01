# 📦 Inventory Management Web Application on AWS

This repository contains the source code and infrastructure setup for a **cloud-native, scalable, and secure 3-tier Inventory Management Web Application**. Built using **Next.js**, **Node.js**, **PostgreSQL**, and deployed via **Amazon Web Services (AWS)**, this project is a modern solution tailored for enterprise-level inventory operations.

---

## 🚀 Project Overview

The application provides a seamless inventory management experience with key features such as product listings, real-time analytics, user permissions, and secure data handling. The architecture ensures **scalability**, **high availability**, and **cost-efficiency** by leveraging AWS services such as EC2, RDS, Amplify, Auto Scaling, Load Balancer, and CloudWatch.

---

## 🖼️ AWS Architecture Design

![AWS Cloud Architecture](https://github.com/user-attachments/assets/1164c585-a3d2-46dc-8956-b0754580ea2a)


---

## ⚙️ Tech Stack

### Frontend
- **Framework:** [Next.js](https://nextjs.org/)
- **Hosting:** AWS Amplify
- **CI/CD:** GitHub → Amplify (Auto-deploy on push)

### Backend
- **Runtime:** Node.js (Express.js)
- **Server Hosting:** Amazon EC2
- **API Gateway:** AWS API Gateway (HTTPS to EC2 backend)

### Database
- **Type:** Amazon RDS (PostgreSQL)
- **Access:** Private subnet (via EC2)

---

## 🌐 AWS Cloud Infrastructure

| Service             | Purpose                                  |
|---------------------|------------------------------------------|
| **VPC & Subnets**   | Network isolation (public/private setup) |
| **EC2**             | Hosting Node.js backend                  |
| **RDS (PostgreSQL)**| Persistent relational database           |
| **Amplify**         | Hosting Next.js frontend                 |
| **S3 Bucket**       | Static file and asset storage            |
| **ALB**             | Load balancing across multiple EC2s      |
| **Auto Scaling**    | Dynamic horizontal scalability           |
| **CloudWatch**      | Monitoring & logging                     |

---

## 🎯 Key Features

- 📋 **Inventory Tracking**: Manage products with stock, price, and rating data.
- 📊 **Dashboard & Analytics**: Real-time data visualization for sales and purchases.
- 🔐 **Secure Backend**: API Gateway + Private RDS Subnet architecture.
- 🌀 **Auto Scaling**: Handle traffic spikes dynamically.
- 🔍 **Monitoring**: Centralized logs and metrics with CloudWatch.
- ♻️ **Continuous Deployment**: GitHub integrated CI/CD with Amplify.

---

## 🧰 Setup Instructions

To run the project locally:

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   ```

2. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   ```

3. **Start backend server**
   ```bash
   npm start
   ```

4. **Install frontend dependencies**
   ```bash
   cd frontend
   npm install
   ```

5. **Run frontend**
   ```bash
   npm run dev
   ```

6. **Access the app**
   ```
   http://localhost:3000
   ```

> 📝 Ensure `.env` files are correctly configured for both frontend and backend environments.

---

## 📊 Monitoring Dashboard

The application is integrated with AWS CloudWatch for:
- EC2 and RDS CPU usage
- API Gateway metrics
- Auto Scaling group events
- Custom dashboards and alarms

---

## 🧑‍💻 Contributors

- **Sachin Mhetre**
- **Mihir Hebalkar**
- **Onkar Mendhapurakar**

---

## 📄 License

This project is for educational purposes and licensed under [MIT License](LICENSE).

