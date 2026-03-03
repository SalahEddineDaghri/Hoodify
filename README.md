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

<img width="1366" height="768" alt="Screenshot 2026-03-02 150852" src="https://github.com/user-attachments/assets/08a08ab1-d78d-4b97-873e-ca462de80ae2" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 151012" src="https://github.com/user-attachments/assets/459333c1-078b-423b-9574-c9ffc84a12c5" />


### 🛒 Cart

<img width="1366" height="768" alt="Screenshot 2026-03-02 151018" src="https://github.com/user-attachments/assets/16c42c99-96ca-42b6-a3bf-c9369612ab9f" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 151216" src="https://github.com/user-attachments/assets/950dfd68-9880-483b-9e68-c0097804c351" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 151224" src="https://github.com/user-attachments/assets/3d98891e-caab-4ad1-b590-47c1b1f82d1e" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 151247" src="https://github.com/user-attachments/assets/a2a8c4ab-f9d3-4e77-971a-ecc7f7c2e5ed" />



### 🛠️ Admin Dashboard

<img width="1366" height="768" alt="Screenshot 2026-03-02 151401" src="https://github.com/user-attachments/assets/e815ed89-8da0-4587-8044-0e75f7057290" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 151410" src="https://github.com/user-attachments/assets/bb738087-a0fc-47f1-826a-a74f2cf140e3" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 145924" src="https://github.com/user-attachments/assets/b35bdd71-d06e-48bd-90bb-23d2498d4d58" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 150237" src="https://github.com/user-attachments/assets/a705270c-0cb6-4c76-b57e-8b9c983dcc98" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 150243" src="https://github.com/user-attachments/assets/bd30fe01-7d0d-4335-84c9-b92b40ba66df" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 150402" src="https://github.com/user-attachments/assets/396193db-f16d-425f-8719-f5444dfd5f28" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 150419" src="https://github.com/user-attachments/assets/29c33149-af3a-4d2a-acae-d715f1c26ea6" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 150433" src="https://github.com/user-attachments/assets/1f790755-d97a-4256-9a61-b6a031986bc3" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 150601" src="https://github.com/user-attachments/assets/41cbc05f-f07c-43d6-8c49-95d98c8473f9" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 150620" src="https://github.com/user-attachments/assets/f679469a-2a69-4721-8c71-76072cbb3a38" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 150658" src="https://github.com/user-attachments/assets/92c5260c-aeca-4e62-a983-5b9ce14d8521" />
<img width="1366" height="768" alt="Screenshot 2026-03-02 150705" src="https://github.com/user-attachments/assets/1ff1bb3b-f345-453d-9512-cd25d7262de0" />











---

## 🔒 Access

This application is private and not publicly accessible.
It is developed for internal testing and portfolio demonstration purposes only.

