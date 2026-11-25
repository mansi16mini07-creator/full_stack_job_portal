# MERN Job Portal

A runnable medium-level Job Portal built with MongoDB, Express, React (Vite), and Node.js.

## Features
- Register/login as a **job seeker** or **recruiter**
- JWT authentication and protected routes
- Recruiters can create and delete their own job posts
- Job seekers can browse/search jobs and apply with a short cover note
- Users can view their applications; recruiters can view applicants for their jobs

## Requirements
- Node.js 18+
- MongoDB running locally, or a MongoDB Atlas connection string

## 1. Start the backend
```bash
cd server
cp .env.example .env
npm install
npm run dev
```
Edit `server/.env` and set `MONGO_URI` and a long `JWT_SECRET`.

Backend runs at `http://localhost:5000`.

## 2. Start the frontend (new terminal)
```bash
cd client
npm install
npm run dev
```
Open the URL printed by Vite (usually `http://localhost:5173`).

## Demo workflow
1. Register one account with role **recruiter** and create a job.
2. Register another account with role **job seeker** and apply.
3. Log in as the recruiter to see applicants.

## Notes
- This is a learning project, not production-hardened.
- For production, add email verification, password reset, rate limiting, input validation, pagination, file storage for resumes, and stronger deployment secrets.
