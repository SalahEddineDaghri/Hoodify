🛍️ Hoodify — Full-Stack E-Commerce Platform

production-ready full-stack e-commerce application featuring a customer storefront and a powerful admin dashboard.

---

## 📋 Table of Contents

* [Overview](#-overview)
* [Tech Stack](#-tech-stack)
* [Features](#-features)
* [System Architecture](#-system-architecture)
* [Docker Setup](#-docker-setup)
* [Admin Dashboard](#-admin-dashboard)
* [Screenshots](#-screenshots)
* [Access](#-access)

---

## 🌟 Overview

** Hoodify ** is a modern full-stack e-commerce web application built to simulate a real-world online store environment.

It includes:

* A customer-facing storefront
* Secure authentication system
* Order management
* Admin dashboard
* Fully containerized infrastructure using Docker

The application follows clean architecture principles and separation of concerns between frontend and backend.

---

## 🧰 Tech Stack

### Frontend

| Technology         | Purpose           |
| ------------------ | ----------------- |
| React + TypeScript | UI framework      |
| Vite               | Build tool        |
| Tailwind CSS       | Styling           |
| Redux Toolkit      | State management  |
| React Router       | Routing           |
| Axios              | API communication |

### Backend

| Technology        | Purpose               |
| ----------------- | --------------------- |
| Node.js + Express | REST API server       |
| Prisma ORM        | Database access layer |
| MySQL 8           | Relational database   |
| JWT               | Authentication        |
| Bcrypt            | Password hashing      |
| Multer            | File uploads          |
| Nodemailer        | Email notifications   |
| Helmet + CORS     | Security              |

### Infrastructure

| Technology       | Purpose               |
| ---------------- | --------------------- |
| Docker           | Containerization      |
| Docker Compose   | Service orchestration |
| Nginx (optional) | Reverse proxy         |

---

## ✨ Features

### 🛒 Storefront

* Product catalog with filtering
* Product detail page
* Image gallery support
* Cart system
* Multi-step checkout flow
* Order confirmation

### 🔐 Authentication

* Secure admin login using JWT
* Protected admin routes
* Password hashing with Bcrypt
* Token-based authorization

### 📦 Order & Product Management

* Product CRUD operations
* Category management
* Order status updates
* Customer data management
* Image upload support via Multer
* Email notifications via Nodemailer

---

## 🏗️ System Architecture

```
project-root/
│
├── Backend/                # Node.js + Express API
│   ├── prisma/
│   │   ├── schema.prisma
│   │   └── seed.js
│   ├── src/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── routes/
│   │   └── utils/
│   ├── uploads/
│   ├── server.js
│   └── Dockerfile
│
├── frontend/               # React + Vite SPA
│   ├── components/
│   ├── pages/
│   ├── store/
│   └── Dockerfile
│
└── docker-compose.yml
```

Frontend communicates with backend through RESTful APIs.
Prisma manages database queries and schema.
JWT secures protected routes.

---

## 🐳 Docker Setup

The full application runs in isolated containers:

* Frontend container
* Backend API container
* MySQL database container

### Start all services

```bash
docker compose up -d --build
```

### Stop services

```bash
docker compose down
```

---

## 🖥️ Admin Dashboard

Accessible via `/admin`.

Admin capabilities:

* Manage products (create, update, delete)
* Manage categories
* View and update orders
* Monitor customers
* Upload product images
* View analytics data

---

## 📸 Screenshots

### 🏠 Home Page

<img width="1348" height="530" alt="Screenshot 2026-03-02 150809" src="https://github.com/user-attachments/assets/795d86df-0bd8-438d-8a7a-d190d0578a88" />
<img width="1346" height="719" alt="Screenshot 2026-03-02 150831" src="https://github.com/user-attachments/assets/1afc79e1-b188-4bbc-ad68-e67257c4aed3" />



### 📦 Product Page

![Product](./screenshots/product.png)

### 🛒 Cart

![Cart](./screenshots/cart.png)

### 🛠️ Admin Dashboard

![Admin](./screenshots/admin.png)

---

## 🔒 Access

This application is private and not publicly accessible.
It is developed for internal testing and portfolio demonstration purposes only.

---

<div align="center">
  Built with 💻 by <strong>Salah-Eddine Daghri</strong>
</div>
