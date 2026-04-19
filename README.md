# Dealerships Review Portal - Fullstack Software Developer Capstone Project

## 📌 Project Name
Dealerships Review Portal - Fullstack Software Developer Capstone Project

## 📁 Repository Name
Fullstack_Dev_Capstone_Project

## 🔗 GitHub Repository URL
https://github.com/SiRipo92/Fullstack_Dev_Capstone_Project

---

## 📖 Project Overview

This project is the final capstone for the **Fullstack Software Developer Certification**.  
It is a full-stack web application designed for a national car dealership network, allowing users to:

- View dealership details across different states
- Read customer reviews
- Submit reviews (for logged-in users)
- Analyze sentiment of reviews using AI

---

## 🎯 Objectives

- Build a complete full-stack application using modern technologies
- Implement microservices architecture
- Integrate sentiment analysis using cloud services
- Deploy the application with CI/CD pipelines

---

## 🚀 Key Features

### 👤 Anonymous Users
- View dealerships
- Filter dealerships by state
- Read reviews

### 🔐 Authorized Users
- Login/Register
- Submit reviews
- View personal reviews

### 🛠 Admin Users
- Manage dealerships
- Add car makes and models
- Access Django admin panel

### 🤖 Sentiment Analysis
- Reviews are analyzed as:
  - Positive
  - Negative
  - Neutral

---

## 🧰 Technologies Used

### Backend
- Django (Python)
- Node.js (Express)

### Frontend
- React.js

### Database
- MongoDB (Dealers & Reviews)
- SQLite (Django models)

### DevOps & Deployment
- Docker
- IBM Cloud Code Engine
- GitHub Actions (CI/CD)

---

## 🏗 System Architecture

1. **Django Backend**
   - Handles authentication and UI routing
   - Communicates with Node backend

2. **Node.js Microservice**
   - Handles dealer & review data
   - Connected to MongoDB

3. **Sentiment Analyzer**
   - Deployed on IBM Cloud
   - Analyzes review text

4. **Frontend (React)**
   - Displays UI components
   - Communicates with Django APIs

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository
```bash
git clone https://github.com/SiRipo92/Fullstack_Dev_Capstone_Project
cd Fullstack_Dev_Capstone_Project
