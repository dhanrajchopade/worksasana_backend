# ✅ Backend Project Feature Checklist

A full-featured task and project management backend built using **Node.js**, **Express**, **MongoDB**, and **JWT authentication**.

---

## 🚀 Setup

- [x] `.env` support using `dotenv`
- [x] Express server setup
- [x] MongoDB connection (`initializeDatabase`)

---

## 🔐 Authentication

- [x] `POST /auth/signup` – Create a new user (with hashed password)
- [x] `POST /auth/login` – Login with email/password and return JWT token
- [x] `GET /auth/me` – Get logged-in user details (using JWT)

---

## 🧠 Middleware

- [x] `verifyJWT` – Protect routes using JWT token
- [x] `cors` middleware – Enabled with open origin

---

## 📁 Models

- [x] `User`
- [x] `Team`
- [x] `Task`
- [x] `Tag`
- [x] `Project`

---

## ✅ Tasks API

- [x] `POST /tasks` – Create new task
- [x] `GET /tasks` – Filter/search tasks by:
  - Team
  - Owner
  - Tags
  - Project
  - Status
- [x] `PUT /tasks/:id` – Update a task
- [x] `DELETE /tasks/:id` – Delete a task

---

## 👥 Teams API

- [x] `POST /teams` – Create a team
- [x] `GET /teams` – Get all teams

---

## 📌 Projects API

- [x] `POST /projects` – Create a project
- [x] `GET /projects` – Get all projects

---

## 🏷️ Tags API

- [x] `POST /tags` – Create a tag
- [x] `GET /tags` – Get all tags

---

## 📊 Reporting APIs

- [x] `GET /report/last-week` – Tasks completed in the last 7 days
- [x] `GET /report/pending` – Total pending work (in days)
- [x] `GET /report/closed-tasks` – Aggregated report by team, owner, and project

---

## 🧪 Optional Features (commented/seeding)

- [ ] JSON file-based data seeding for:
  - Projects
  - Tags
  - Tasks
  - Teams
  - Users
- [ ] Enable by uncommenting seed logic

---

## ⚙️ Technologies Used

- Node.js
- Express.js
- MongoDB (with Mongoose)
- JWT for authentication
- bcrypt for password hashing
- dotenv for environment variables
- cors for cross-origin requests
