# 🚀 Jobshala - Full-Stack MERN Job Portal

Welcome to **Jobshala**—a robust, production-ready full-stack job portal application built using the MERN stack. This project showcases proficiency in modern web development best practices, including role-based access control, secure authentication, and cloud deployment.

## 🌟 Quick Access (Live & Code)

| Type | Badge | URL |
| :--- | :--- | :--- |
| **Live Application** | [![Deployed on Vercel](https://img.shields.io/badge/LIVE%20APP-VERCEL-21759b?style=for-the-badge&logo=vercel)](https://jobshala-eight.vercel.app) | `https://jobshala-eight.vercel.app` |
| **Current GitHub Repo** | [![GitHub Repository](https://img.shields.io/badge/Code-GitHub-100000?style=for-the-badge&logo=github)](https://github.com/aarjav-jain151/jobshala) | `https://github.com/aarjav-jain151/jobshala` |
| **Backend API** | [![API on Render](https://img.shields.io/badge/API-RENDER-46E3B7?style=for-the-badge&logo=render)](https://jobshala-backend-0hf7.onrender.com) | `https://jobshala-backend-0hf7.onrender.com` |

---

## ✨ Key Features & Functionalities

The application implements comprehensive features for both job seekers and recruiters:

### User Management & Authentication
- **Secure Auth:** JWT-based user authentication and authorization.
- **Role-Based Access:** Separate roles for **Job Seekers** (`student`) and **Recruiters** (`recruiter`).
- **Protected Routes:** Frontend and Backend routes are protected based on user roles.

### Core Features
- **Job Browsing & Filter:** View, search, and filter job listings by title, category, and location.
- **Job Application:** Apply to jobs with **Resume Upload** functionality.
- **Recruiter Dashboard:** Recruiters can post, edit, and delete job listings.
- **Applicant Tracking:** Recruiters can view all applicants for their jobs and update their application status.

---

## 🛠️ Technology Stack

| Category | Technologies Used |
| :--- | :--- |
| **Frontend** | **ReactJS** (with Vite), **Redux Toolkit** (State Management), **Tailwind CSS**, **shadcn/ui** |
| **Backend** | **Node.js**, **Express.js** |
| **Database** | **MongoDB** (using **Mongoose** ORM) |
| **Deployment** | **Vercel** (Frontend), **Render** (Backend), **MongoDB Atlas** (Cloud DB) |
| **Utilities** | **JSON Web Tokens (JWT)**, **`dotenv`**, **`multer`** (for file uploads). |

---

## ⚙️ Installation & Setup (Local Development)

Follow these steps to clone the repository and run the project locally.

1.  **Clone the Repository:**

    First, navigate to the folder where you want to store your projects, and then clone the repository.
    ```bash
    # 1. Clone the project (downloads the code)
    git clone [https://github.com/aarjav-jain151/jobshala.git](https://github.com/aarjav-jain151/jobshala.git)
    
    # 2. Change directory into the new project folder
    cd jobshala
    ```

2.  **Install Dependencies (Backend & Frontend):**

    You need to install packages for both the server and the client.
    ```bash
    # Install backend dependencies
    cd backend
    npm install
    
    # Install frontend dependencies (navigate back, then into frontend)
    cd ../frontend
    npm install
    ```

3.  **Setup Environment Variables:**

    Create a file named **`.env`** inside the **`backend`** directory. Add your specific credentials here. **Note:** The `MONGO_URI` below should be the working string from your MongoDB Atlas setup (including any URL-encoding for the password).
    
    ```env
    # Replace these placeholders with your actual secrets
    MONGO_URI=mongodb://<YOUR_ATLAS_USER>:<YOUR_URL_ENCODED_PASS>@<YOUR_CLUSTER_URL>/jobportal_app
    JWT_SECRET_KEY=A_NEW_LONG_RANDOM_SECRET_KEY_FOR_LOCAL_DEV
    
    # Local Development Settings
    NODE_ENV=development
    PORT=8000
    FRONTEND_URL=http://localhost:5173
    ```

4.  **Run the Project:**

    Open two separate terminals/tabs in VS Code to run the frontend and backend simultaneously.
    ```bash
    # Terminal 1: Start Backend Server
    cd backend
    npm run dev
    
    # Terminal 2: Start Frontend Application
    cd frontend
    npm run dev
    ```

The application will be live in your browser at **`http://localhost:5173`**.
