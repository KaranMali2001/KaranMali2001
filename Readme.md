<!-- HEADER / INTRO -->

<div align="center">
  <h1>Hi there, I'm <strong>Karan Mali</strong> 👋</h1>
  <p>Backend Developer • API / Microservices • Go | Node.js | TypeScript</p>
</div>

---

## 🔭 About Me

* I build scalable and maintainable backend systems powered by clean architecture and best practices.
* Strong with databases (relational & NoSQL), authentication & authorization, performance optimization, and error handling.
* Always learning new tools and techniques — currently exploring microservices in Go, advanced testing, and cloud deployment.

---

## 🛠 Tech Stack

| Area            | Tools & Languages                                       |
| --------------- | ------------------------------------------------------- |
| Languages       | Go, TypeScript (Node.js), JavaScript                    |
| Frameworks      | Express, Fastify, Gin                                   |
| Databases       | PostgreSQL, MongoDB, Redis                              |
| Tools & Infra   | Docker, JWT, REST APIs, Git, Linux                      |
| Testing / CI/CD | Jest / Mocha, Supertest, GitHub Actions, Docker Compose |

---

## 📁 My Projects

Here are some backend-focused projects of mine. Click to explore their code 🔍

| Project               | What It Does / Key Features                                                       |
| --------------------- | --------------------------------------------------------------------------------- |
| **Mini-Ride-Booking** | Ride-booking lifecycle: booking, driver/rider matching, JWT auth, booking states. |
| **Finance-Tracker**   | CRUD operations, transaction summaries, category filtering, secure APIs.          |
| **Habit-Tracker**     | Schedule-based tasks, reminders, user profiles, background jobs.                  |
| **MatchUp**           | Tournament / bracket logic, validations, REST endpoints, error handling.          |

---

## 🚀 Code Sample

Here’s a snippet showing how I handle error responses in Node.js + TypeScript — clean, consistent, and JSON-API style:

```ts
// src/middleware/errorHandler.ts
import { Request, Response, NextFunction } from 'express';

interface AppError extends Error {
  statusCode?: number;
  isOperational?: boolean;
}

function errorHandler(
  err: AppError,
  req: Request,
  res: Response,
  next: NextFunction
) {
  console.error(`[ERROR] ${err.message}`, err);

  const statusCode = err.statusCode ?? 500;
  const message = err.isOperational
    ? err.message
    : 'Something went wrong';

  res.status(statusCode).json({
    success: false,
    error: {
      message,
    }
  });
}

export default errorHandler;
```

---

## 📈 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=KaranMali2001&show_icons=true&theme=dark&hide=issues" />
</div>

---

## 🌱 What I’m Learning & Exploring

* Building microservices in Go
* Implementing robust integration / end-to-end tests
* Cloud native deployment (Docker, Kubernetes, maybe AWS/GCP)
* Message queues / event-driven architectures

---

## 📫 Let’s Connect

* 🌐 Portfolio / Blog: *(add link here if you have one)*
* 💼 LinkedIn: [karan5599](https://www.linkedin.com/in/karan5599)
* 📧 Email: *(add email if you’d like to share)*

---

Thank you for visiting my profile!
Let’s build something awesome together 🤝
