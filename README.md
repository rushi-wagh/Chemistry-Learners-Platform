# Chemistry Learners Platform

A full-stack learning management system built for chemistry students. The platform allows students to access courses, watch lecture videos, download study materials, track learning progress, and purchase premium courses. It also includes a complete admin panel for managing courses, content, study materials, and enrollments.

---

# Features

## Student

- Interactive dashboard with learning progress
- Search and filter chemistry courses and batches
- Premium lecture video player
- Download lesson-wise PDFs and study materials
- Free study material section
- Automatic course progress tracking
- Razorpay payment integration
- Email verification and password reset
- User profile management

## Admin

- Dashboard with enrollment and revenue statistics
- Create, edit and publish courses
- Manage chapters and lessons
- Upload PDFs and documents using Cloudinary
- Manage free study materials
- Monitor payments and student enrollments

---

# Tech Stack

## Frontend

- React 19 (Vite)
- Tailwind CSS v4
- React Router v7
- Axios
- GSAP
- React PDF
- Lucide React
- React Icons
- React Hot Toast
- React Loader Spinner

## Backend

- Node.js
- Express.js
- MongoDB
- Mongoose
- Cloudinary
- Resend
- Razorpay
- JWT Authentication
- BcryptJS
- Multer
- UUID
- DayJS

---

# Project Structure

```text
Chemistry-Learners-Platform
│
├── Backend
│   ├── src
│   │   ├── controllers
│   │   ├── db
│   │   ├── middleware
│   │   ├── models
│   │   ├── routes
│   │   └── utils
│   ├── index.js
│   ├── .env.example
│   └── package.json
│
├── Frontend
│   ├── public
│   ├── src
│   │   ├── assets
│   │   ├── components
│   │   ├── Context
│   │   ├── pages
│   │   ├── utils
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

---

# Getting Started

## Prerequisites

- Node.js (v18 or above)
- MongoDB Atlas or Local MongoDB
- Cloudinary Account
- Resend Account
- Razorpay Account

---

# Backend Setup

```bash
cd Backend
```

Install dependencies

```bash
npm install
```

Create a `.env` file.

```env
PORT=8000
BASE_URL=http://localhost:8000
FRONTEND_URL=http://localhost:5173

MONGO_URI=your_mongodb_connection_string

ACCESS_TOKEN_SECRET=your_access_token_secret
REFRESH_TOKEN_SECRET=your_refresh_token_secret
ACCESS_TOKEN_EXPIRY=1d
REFRESH_TOKEN_EXPIRY=10d

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

RESEND_API_KEY=your_resend_api_key

RAZORPAY_KEY_ID=your_key_id
RAZORPAY_KEY_SECRET=your_key_secret
```

Start the backend server.

```bash
npm run dev
```

Server runs at

```
http://localhost:8000
```

---

# Frontend Setup

```bash
cd Frontend
```

Install dependencies.

```bash
npm install
```

Run the development server.

```bash
npm run dev
```

Frontend runs at

```
http://localhost:5173
```

---

# API Routes

| Module | Route |
|---------|-------|
| Auth | `/api/v1/auth` |
| Users | `/api/v1/users` |
| Courses | `/api/v1/courses` |
| Chapters | `/api/v1/chapters` |
| Lessons | `/api/v1/lessons` |
| Materials | `/api/v1/materials` |
| Free Materials | `/api/v1/free-materials` |
| Course Progress | `/api/v1/course-progress` |
| Enrollments | `/api/v1/enrollments` |
| Payments | `/api/v1/payments` |
| Health Check | `/api/v1/health` |

---


