
# 💼 Job Portal

**Job Portal** is a full-stack web application designed to connect job seekers with employers. It allows users to create accounts, browse job listings, apply for jobs, and manage applications. Employers can post new jobs, view applicants, and manage company profiles. The project includes authentication, authorization, and file uploads for resumes and logos.

---

## 🚀 Features

### 👤 User Roles
- **Job Seekers**: Sign up, view and apply for jobs, manage profile.
- **Companies**: Post job listings, view applicant information.
- **Admins**: Access and manage users, jobs, and companies.

### 📄 Job Application System
- Users can browse and filter jobs.
- Companies can post and edit job listings.
- Applications are stored with resume uploads.

### 🔐 Authentication & Authorization
- JWT-based user login and secure access to protected routes.
- Middleware-based role checking for admin, user, and company.

### 📁 Resume & Logo Uploads
- Uses Multer middleware for handling file uploads (e.g., resumes, logos).

---

## 🛠️ Tech Stack

| Layer     | Technology          | Description                            |
|-----------|---------------------|----------------------------------------|
| Frontend  | React.js (assumed)  | Client-side interface (if present)     |
| Backend   | Node.js, Express.js | REST API and business logic            |
| Database  | MongoDB             | Stores users, jobs, applications       |
| Auth      | JWT                 | Token-based authentication             |
| Uploads   | Multer              | Middleware for file uploads            |

---

## 📁 Folder Structure

```
Job-Portal-main/
├── backend/
│   ├── controllers/        # Request handlers (application, company, job, user)
│   ├── middlewares/        # Role/authentication, file uploads
│   ├── models/             # MongoDB schemas
│   ├── routes/             # API endpoints
│   ├── package.json        # Node dependencies
│   └── index.js            # App entry point
└── frontend/ (if applicable)
```

---

## ⚙️ Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/job-portal.git
cd Job-Portal-main
```

### 2. Backend Setup
```bash
cd backend
npm install
```
Create a `.env` file with the following variables:
```
MONGODB_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
```

Then start the backend server:
```bash
node index.js
```

### 3. Frontend Setup (Optional)
If the frontend exists, navigate to the `frontend/` directory and run:
```bash
npm install
npm start
```

### 4. Open in browser
Visit: `http://localhost:3000`

---

## 📄 License

This project currently has no license.

---

## 🙌 Acknowledgments

- Inspired by job platforms like LinkedIn and Indeed.
