# 🛡️ SmartShield AI

### Multi-Agent Investigation & Risk Explanation System

<p align="center">
  <strong>Version:</strong> v0.1.0 &nbsp;|&nbsp;
  <strong>Development Stage:</strong> Beta
</p>

<p align="center">
  <strong>Status:</strong> 🚧 Actively Under Development
</p>

> ⚠️ **Development Notice:** SmartShield AI is currently in its beta development stage. The application is deployed and functional, but bugs, incomplete features, and unexpected behavior may occur. The system is undergoing continuous development, testing, and improvement. It is not yet considered a stable production release.

SmartShield AI is an intelligent cybersecurity platform designed to help users identify online scams, analyze suspicious messages and URLs, assess fraud risks, and take appropriate actions to protect themselves.

The platform combines automated scam detection, risk scoring, evidence analysis, and recovery assistance to provide users with actionable cybersecurity insights.

---

## 📊 Project Status

| Attribute | Details |
|---|---|
| Project Name | SmartShield AI |
| Current Version | v0.1.0 |
| Development Stage | Beta |
| Project Status | Actively Under Development |
| Deployment Status | Deployed |
| Frontend | Vercel |
| Backend | Render |
| Database | Supabase PostgreSQL |
| Stability | Testing and debugging ongoing |

---

## 🌐 Live Application

- **Frontend:** https://smartshield-ai-six.vercel.app
- **Backend API:** https://smartshield-ai-c1n1.onrender.com
- **GitHub Repository:** https://github.com/dileep9611marathi/smartshield-ai

---

## 📌 Project Overview

Online scams, phishing attacks, fraudulent payment requests, and impersonation schemes are becoming increasingly common.

SmartShield AI aims to help users make safer digital decisions by analyzing suspicious content and identifying potential scam indicators.

The system uses a structured investigation pipeline to analyze evidence, identify risk indicators, generate risk scores, and provide explanations that help users understand why something may be suspicious.

---

## ✨ Features

### 🔍 Scam Investigation
- Analyze suspicious messages and text.
- Identify potential scam indicators.
- Detect urgency tactics and account threats.
- Evaluate suspicious links and phishing patterns.
- Generate investigation results with explanations.

### ⚠️ Risk Assessment
- Automated risk scoring.
- Risk classification levels.
- Confidence estimation.
- Evidence-based risk explanations.
- Identification of suspicious behavioral patterns.

### 🛡️ Before-You-Pay Protection
- Evaluate suspicious payment requests.
- Identify potential fraud warning signs.
- Help users assess risks before making payments.

### 🚨 Emergency Assistance
- Emergency fraud triage.
- Guidance for users experiencing financial scams.
- Emergency contact information and assistance workflows.

### 📋 Scam Pattern Detection
- Database of known scam patterns.
- Identification of common fraud techniques.
- Scam indicator analysis.

### 🔄 Recovery Assistance
- Recovery case management.
- Track the status of reported scams.
- Store recovery notes and updates.
- Organize information related to fraud incidents.

### 🔐 Authentication
- User registration.
- Login authentication.
- JWT-based authentication.
- Protected application functionality.

---

## 🏗️ System Architecture

SmartShield AI follows a full-stack architecture consisting of a React frontend, Node.js backend, and PostgreSQL database.

```text
                    ┌──────────────────────┐
                    │       User           │
                    │   Web Browser        │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │  React + Vite        │
                    │  Frontend            │
                    │  Hosted on Vercel    │
                    └──────────┬───────────┘
                               │
                         REST API Requests
                               │
                               ▼
                    ┌──────────────────────┐
                    │  Node.js + Express   │
                    │  TypeScript Backend  │
                    │  Hosted on Render    │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │  PostgreSQL Database │
                    │  Hosted on Supabase  │
                    └──────────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend
- React
- TypeScript
- Vite
- HTML5
- CSS3

### Backend
- Node.js
- Express.js
- TypeScript
- REST API
- JWT Authentication

### Database
- PostgreSQL
- Supabase

### Deployment & DevOps
- Git
- GitHub
- Vercel
- Render
- Supabase

---

## 📂 Project Structure

```text
smartshield-ai/
│
├── backend/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── database/
│   │   ├── middleware/
│   │   ├── repositories/
│   │   ├── routes/
│   │   ├── services/
│   │   └── server.ts
│   │
│   ├── package.json
│   └── tsconfig.json
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── types/
│   │   └── ...
│   │
│   ├── package.json
│   ├── vite.config.ts
│   └── vercel.json
│
├── database/
│   ├── migrations/
│   │   └── 001_initial_schema.sql
│   │
│   └── seeds/
│       └── 001_seed_scam_patterns.sql
│
├── package.json
├── README.md
└── .gitignore
```

---

## ⚙️ Installation and Setup

### Prerequisites

Install the following before running the project locally:

- Node.js
- npm
- Git
- PostgreSQL database or Supabase account

### 1. Clone the Repository

```bash
git clone https://github.com/dileep9611marathi/smartshield-ai.git
```

Navigate into the project directory:

```bash
cd smartshield-ai
```

### 2. Install Dependencies

Install the root dependencies:

```bash
npm install
```

Install backend dependencies:

```bash
cd backend
npm install
```

Install frontend dependencies:

```bash
cd ../frontend
npm install
```

### 3. Configure Environment Variables

Create an environment file for the backend.

```text
backend/.env
```

Configure the required variables:

```env
NODE_ENV=development
PORT=5000

DATABASE_URL=your_postgresql_connection_string

JWT_SECRET=your_secure_jwt_secret

CORS_ORIGIN=http://localhost:5173
```

Create the frontend environment file:

```text
frontend/.env
```

```env
VITE_API_BASE_URL=http://localhost:5000/api/v1
```

**Important:** Never commit `.env` files, passwords, API keys, or authentication secrets to GitHub.

### 4. Configure the Database

Connect your PostgreSQL database.

Run the initial database migration:

```text
database/migrations/001_initial_schema.sql
```

Run the seed data:

```text
database/seeds/001_seed_scam_patterns.sql
```

These scripts create the database schema and populate the initial scam pattern data.

### 5. Start the Backend

Navigate to the backend:

```bash
cd backend
```

Start the development server using the development script configured in `backend/package.json`.

The backend will run on:

```text
http://localhost:5000
```

### 6. Start the Frontend

Navigate to the frontend:

```bash
cd frontend
```

Start the Vite development server:

```bash
npm run dev
```

The frontend will normally be available at:

```text
http://localhost:5173
```

---

## 🔌 API

The backend API uses the following base URL:

```text
/api/v1
```

### Health Check

```http
GET /api/v1/health
```

Example response:

```json
{
  "success": true,
  "status": "healthy",
  "product": "SmartShield AI",
  "version": "1.0.0"
}
```

### Authentication

Authentication endpoints are available under:

```text
/api/v1/auth
```

The system supports user registration and authentication using JWT-based authorization.

---

## 🚀 Deployment

### Frontend — Vercel

The React frontend is deployed using Vercel.

Configuration:

| Setting | Value |
|---|---|
| Framework | Vite |
| Root Directory | `frontend` |
| Build Command | `npm run build` |
| Output Directory | `dist` |

Environment variable:

```env
VITE_API_BASE_URL=https://smartshield-ai-c1n1.onrender.com/api/v1
```

A `vercel.json` configuration is included to support SPA routing and direct page refreshes.

### Backend — Render

The Express backend is deployed using Render.

Configuration:

| Setting | Value |
|---|---|
| Service Type | Web Service |
| Runtime | Node.js |
| Root Directory | `backend` |
| Build Command | `npm install --include=dev && npm run build` |
| Start Command | `npm start` |

Environment variables are configured through the Render dashboard.

### Database — Supabase

Supabase provides the PostgreSQL database used by SmartShield AI.

The backend connects to PostgreSQL using the database connection string configured through environment variables.

---

## 🔒 Security

The project implements:

- JWT-based authentication.
- Environment-based secret management.
- Backend API architecture.
- CORS configuration.
- Database-backed persistence.
- Protected application workflows.

Security configurations and deployment settings should be reviewed before production use.

---

## 🎯 Project Objectives

- Detect suspicious online messages and potential scams.
- Provide understandable explanations of scam indicators.
- Assess digital fraud risks.
- Help users make informed decisions before payments.
- Provide assistance during fraud-related emergencies.
- Organize recovery information for scam victims.
- Promote digital safety and cybersecurity awareness.

---

## 🔮 Future Improvements

- Integration with additional threat intelligence sources.
- Improved AI-based scam classification.
- Advanced URL reputation analysis.
- Image and screenshot-based scam detection.
- Improved multilingual scam detection.
- More sophisticated risk scoring models.
- Enhanced fraud investigation and recovery workflows.
- Analytics dashboard for scam trends.
- Stronger production security and authorization controls.
- Bug fixes and performance improvements.

---

## 🧪 Development Status

SmartShield AI is currently in the **Beta (v0.1.0)** stage.

The application has been deployed and initial functionality has been tested. However, development is ongoing.

Current development activities include:

- Testing all application workflows.
- Fixing bugs and unexpected behavior.
- Improving user experience.
- Refining scam detection and risk scoring.
- Testing API integration.
- Improving security and reliability.
- Preparing for a more stable release.

The deployed application should be considered a testing and development version rather than a fully stable production product.

---

## 👥 Project Information

**Project Name:** SmartShield AI

**Category:** Cybersecurity / Artificial Intelligence / Fraud Detection

**Architecture:** Full-Stack Web Application

**Frontend Deployment:** Vercel

**Backend Deployment:** Render

**Database:** Supabase PostgreSQL

**Version:** v0.1.0

**Development Stage:** Beta

---

## 📜 License

This project was developed as an educational and community-oriented cybersecurity project.

A formal license may be added to the repository if the project is intended for open-source distribution.

---

> SmartShield AI — Empowering users to identify digital threats, understand risks, and take safer actions online.

