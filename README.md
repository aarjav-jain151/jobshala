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

Follow these steps to get the project running on your local machine:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/aarjav-jain151/jobshala.git](https://github.com/aarjav-jain151/jobshala.git)
    cd jobshala-mern
    ```

2.  **Install Dependencies (Backend & Frontend):**
    ```bash
    # Backend
    cd backend
    npm install
    
    # Frontend
    cd ../frontend
    npm install
    ```

3.  **Setup Environment Variables:**
    * Create a file named **`.env`** inside the **`backend`** directory.
    * Add your local configuration:
        ```env
        MONGO_URI=mongodb://aarjavjain151_db_user:K%3FJV85sMUz5nBRzB@rstzftd.mongodb.net/jobportal_app
        JWT_SECRET_KEY=VIBGYOR-Jobshala-S3cur3-K3y-42069-M3RN-Stack-R3nd3r-D3pl0y-Aarjav
        NODE_ENV=development
        PORT=8000
        FRONTEND_URL=http://localhost:5173
        ```

4.  **Run the Project:**
    * **Start Backend** (in one terminal):
        ```bash
        cd backend
        npm run dev
        ```
    * **Start Frontend** (in a new terminal):
        ```bash
        cd frontend
        npm run dev
        ```

The application will be live at `http://localhost:5173`.
