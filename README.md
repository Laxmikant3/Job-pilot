# 🚀 Job-Pilot – AI-Powered Job Application & Resume Screening Platform (MERN Stack)

Welcome to **Job-Pilot**, a comprehensive, full-stack solution designed to automate and enhance the hiring process. This platform enables companies to manage job applications efficiently while offering candidates a smooth, modern experience.  

By leveraging **AI-driven resume screening**, **multi-lingual support**, and **Cloudinary for secure file storage**, Job-Pilot revolutionizes the way recruitment works.

---

## 📋 Table of Contents
- [Introduction](#-introduction)  
- [Features](#-features)  
- [Tech Stack](#-tech-stack)  
- [Project Structure](#-project-structure)  
- [Admin Dashboard](#️-admin-dashboard)  
- [Candidate Experience](#-candidate-experience)  
- [AI Integration](#-ai-integration)  
- [Environment Setup](#-environment-setup)  
- [Deployment](#-deployment)  
- [Contributing](#-contributing)  
- [License](#-license)

---

## 🌟 Introduction
**Job-Pilot** is built to streamline the recruitment process for companies and simplify job applications for candidates.  
Admins can post jobs, review resumes, shortlist candidates, and communicate directly — while candidates can upload resumes, apply instantly, and receive AI-powered feedback.  

Using advanced **AI models** like *Gemini 1.5 Flash* (or any other LLM), the system analyzes resumes, matches them against job requirements, and provides reasoning behind every shortlisting decision.

---

## ✨ Features

### 🧩 Core Functionality
#### 📄 Resume Upload & Parsing
- Upload resumes in **PDF/DOCX** format  
- Automatic parsing of key details (Name, Email, Skills, Experience, Education, Projects)  
- Secure cloud storage via **Cloudinary**

#### 📋 Job Postings for Companies
- Post multiple job openings with titles, skills, experience level, and location  
- Define shortlisting thresholds and track applications easily via MongoDB  

#### 🤖 AI-Driven Resume Matching
- Smart resume evaluation based on skills, experience, and education  
- AI fallback logic for deeper evaluation and reasoning  

#### 💬 Interactive Candidate Chatbot
- Multilingual chatbot for application-related queries  
- AI-driven, human-like interactions for better engagement  

#### 📊 Admin Dashboard
- View, filter, and shortlist resumes with AI-based scoring  
- Transparent shortlisting with **AI explanations**

#### 📨 In-App Messaging
- Send personalized messages to candidates  
- Manage interview notifications and rejections efficiently  

---

## 🛠️ Tech Stack

### **Frontend**
- React.js  
- React Router  
- Axios  
- Formik  
- React-FA Icons  
- Tailwind CSS (if used)  

### **Backend**
- Node.js  
- Express.js  
- MongoDB (Mongoose)  
- JWT Authentication  
- Multer (for file uploads)  
- Cloudinary (for storage)

### **AI / LLM**
- Gemini 1.5 Flash (or equivalent AI model)  
- Multilingual reasoning & text analysis

---

## 🗂️ Project Structure
\`\`\`
Job-Pilot/
├── frontend/                # React.js Frontend
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/                 # Node.js Backend
│   ├── controllers/         # API Controllers
│   ├── models/              # MongoDB Models
│   ├── routes/              # Express Routes
│   ├── middleware/          # Auth Middleware
│   ├── utils/               # Helper Functions
│   ├── config/              # DB and Cloud Config
│   └── server.js
│
├── .env                     # Environment Variables
└── README.md
\`\`\`

---

## 🖥️ Admin Dashboard
The **Admin Dashboard** empowers HR teams to:
- **Manage Job Posts:** Create, update, and delete openings  
- **Review Resumes:** View parsed resumes and AI evaluation scores  
- **Communicate:** Message candidates directly via in-app tools  
- **Analyze Jobs:** Track application stats and shortlisting progress  

---

## 👩‍💻 Candidate Experience
Candidates can:
- Upload their resume (PDF/DOCX)  
- Answer job-specific questions  
- Get **instant AI-based feedback** on matching percentage  
- Receive updates on their application status  

Real-time insights help candidates improve future applications and tailor their resumes better.

---

## 🧠 AI Integration
- Uses **Gemini 1.5 Flash** (or similar LLM) for resume matching  
- Generates shortlisting **scores + reasoning**  
- Supports **multilingual responses** for global inclusivity  

---

## ⚙️ Environment Setup
Create a `.env` file in the `backend/` directory:

\`\`\`env
PORT=5100
MONGO_URL=your_mongodb_url
JWT_SECRET=your_jwt_secret
CLOUD_NAME=your_cloudinary_name
CLOUD_API_KEY=your_cloudinary_key
CLOUD_API_SECRET=your_cloudinary_secret
\`\`\`

Then, install dependencies:
\`\`\`bash
# Backend
cd backend
npm install
npm run dev

# Frontend
cd ../frontend
npm install
npm run dev
\`\`\`

---

## 🚀 Deployment
You can deploy this project on:
- **Frontend:** Vercel / Netlify  
- **Backend:** Render / Railway / AWS / Azure  
- **Database:** MongoDB Atlas  
- **Cloud Storage:** Cloudinary  

---
