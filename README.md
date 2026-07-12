# JobFinder 🚀

## Overview

**JobFinder** is a web-based recruitment management platform designed to simplify and centralize the hiring process.

The application allows companies to publish job offers, manage applications, and track recruitment activities. Candidates can create accounts, browse available job opportunities, apply for positions, and monitor the status of their applications.

The platform provides dedicated interfaces for three main user roles:

- 👤 Candidate
- 🏢 HR / Recruiter
- 🔐 Administrator

---

# Main Objectives

The main goal of JobFinder is to provide a complete recruitment management solution where:

- The Company can easily publish and manage job offers.
- Candidates can search and apply for jobs.
- HR teams can manage candidates and recruitment processes.
- Administrators can control access, validate HR accounts, and monitor platform statistics.

---

# User Roles and Permissions
| Role | Main Responsibilities |
|------|----------------------|
| Candidate | Browse jobs, apply, manage profile, track applications |
| HR / Recruiter | Manage job offers, review applications, update application status |
| Administrator | Manage users, validate HR accounts, access global statistics |

---

# Features

## 👤 Candidate Features

Candidates can:

- Create an account and authenticate.
- Update personal information.
- Upload and manage their CV.
- Browse available job offers.
- Search and filter jobs by:
  - Category
  - Location
  - Contract type
- Apply for job opportunities.
- Track application status:
  - Pending
  - Accepted
  - Rejected

---

## 🏢 HR / Recruiter Features

HR users can:

- Create an HR account.
- Wait for administrator approval.
- Login after account validation.
- Create, update, and delete job offers.
- View received applications.
- Review candidate profiles.
- Accept or reject applications.
- Manage recruitment activities.

---

## 🔐 Administrator Features

Administrators can:

- Login with administrator privileges.
- Approve or reject HR registration requests.
- Manage users and access rights.
- Access an interactive dashboard containing:

  - Number of published job offers
  - Number of applications
  - Acceptance rate
  - Active candidates
  - Active HR users

- Monitor platform activities.

---

# System Architecture

JobFinder is divided into two main applications:

```
JobFinder/

│
├── backend/
│   ├── Node.js
│   ├── Express.js
│   ├── REST API
|
├── Database
│
├── frontend/
│   ├── React.js
│   ├── User Interface
│   └── API Integration
│
└── README.md
```

---

# Technologies

## Backend
- Node.js
- Express.js
- REST API
- JWT Authentication
- Database (MongoDB)
- bcrypt
- dotenv

## Frontend
- React.js
- React Router
- Axios
- Bootstrap / Tailwind CSS / Material UI
- Chart.js

---

# Installation and Setup

## Clone Repository

```bash
git clone https://github.com/ouelhezi/JobFinderProject.git

cd jobfinderproject
```

---

# Backend Setup

Navigate to backend folder:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

Create a `.env` file:

```
PORT=5000
MONGO_URL=mongodb://localhost:27017/jobfinder
ACCESS_TOKEN_KEY=abcd
REFRESH_TOKEN_KEY=efgh

EMAIL_SENDER ="your email"
EMAIL_PASSWORD ="your password key" 
```

Start backend server:

```bash
npm run dev or npm start
```

Backend will run on:

```
http://localhost:5000
```

---

# Frontend Setup

Navigate to frontend folder:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start React application:

```bash
npm start
```

Frontend will run on:

```
http://localhost:3000
```

---

# Authentication and Security

The application implements:
- JWT-based authentication
- Role-based authorization
- Protected routes
- Password encryption
- API access control

---

# Application Workflow

```
Candidate
    |
    | Apply for jobs
    ↓
Job Offer
    |
    | Review applications
    ↓
HR Recruiter
    |
    | Accept / Reject
    ↓
Candidate Notification


Administrator
    |
    | Validate HR accounts
    ↓
HR Platform Access
```

---

# Future Improvements

Possible improvements:
- Real-time chat between HR and candidates
- AI-based CV matching
- Advanced analytics
- Mobile application

---

# Live Demo
