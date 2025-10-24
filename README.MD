<h1 align="center">✨ Full-Stack Chat App with Auth & Emails ✨</h1>

![Demo App](/frontend/public/screenshot-for-readme.png)

## 📖 Project Overview

Chatify is a modern, full-stack real-time chat application built with the MERN stack (MongoDB, Express, React, Node.js). It features secure JWT-based authentication, real-time messaging powered by Socket.IO, and a beautiful, responsive UI built with React and Tailwind CSS.

The application allows users to:
- Create accounts and log in securely
- Send and receive messages in real-time
- See who's online/offline
- Upload and share images in conversations
- Receive welcome emails upon signup
- Toggle notification sounds and typing indicators

**Tech Stack:**
- **Frontend:** React, Zustand (state management), Tailwind CSS, DaisyUI
- **Backend:** Node.js, Express, Socket.IO
- **Database:** MongoDB
- **Authentication:** JWT (JSON Web Tokens)
- **File Storage:** Cloudinary (for image uploads)
- **Email Service:** Resend (for welcome emails)
- **Security:** Arcjet (API rate limiting)
- **Deployment:** Frontend on Vercel, Backend on Render

---

## ✨ Highlights:

- 🔐 Custom JWT Authentication (no 3rd-party auth)
- ⚡ Real-time Messaging via Socket.io
- 🟢 Online/Offline Presence Indicators
- 🔔 Notification & Typing Sounds (with toggle)
- 📨 Welcome Emails on Signup (Resend)
- 🗂️ Image Uploads (Cloudinary)
- 🧰 REST API with Node.js & Express
- 🧱 MongoDB for Data Persistence
- 🚦 API Rate-Limiting powered by Arcjet
- 🎨 Beautiful UI with React, Tailwind CSS & DaisyUI
- 🧠 Zustand for State Management
- 🧑‍💻 Git & GitHub Workflow (branches, PRs, merges)
- 🚀 Easy Deployment (free-tier friendly with Sevalla)

---

## 🧪 .env Setup

### Backend (`/backend`)

```bash
PORT=3000
MONGO_URI=your_mongo_uri_here

NODE_ENV=development

JWT_SECRET=your_jwt_secret

RESEND_API_KEY=your_resend_api_key
EMAIL_FROM=your_email_from_address
EMAIL_FROM_NAME=your_email_from_name

CLIENT_URL=http://localhost:5173

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

ARCJET_KEY=your_arcjet_key
ARCJET_ENV=development
```

---

## 🔧 Run the Backend

```bash
cd backend
npm install
npm run dev
```

## 💻 Run the Frontend

```bash
cd frontend
npm install
npm run dev
```

---

## 🚀 Deployment

This project is configured for deployment with:
- **Frontend:** Vercel (or any static hosting service)
- **Backend:** Render (or any Node.js hosting service)

### Frontend Environment Variables (Vercel)

```bash
VITE_API_URL=https://your-backend-url.onrender.com/api
VITE_BACKEND_URL=https://your-backend-url.onrender.com
```

### Backend Environment Variables (Render)

Set `NODE_ENV=production` and update `CLIENT_URL` to your Vercel deployment URL.

**Important Notes:**
- Cookies are configured with `SameSite=None` in production for cross-origin authentication
- CORS is configured to allow requests from your frontend domain
- The backend serves the built frontend files when deployed on a single server

---

## 📝 License

This project is open source and available under the ISC License.
