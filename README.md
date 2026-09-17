# 🛒 MERN E-Commerce Platform

A full-stack e-commerce MVP built with the **MERN stack** (MongoDB, Express, React, Node.js), featuring a customer storefront, authentication, product management, shopping cart, orders, wishlist, invoices, real-time notifications, and an admin dashboard.

🌐 **Live Demo:** https://react-sooty-eta.vercel.app/

---

## ✨ Features

### 🛍️ Customer Space

* Responsive e-commerce storefront
* User registration and authentication
* Login / Logout
* Forgot and reset password
* Product catalog
* Product search
* Product filtering and sorting
* Product details and image gallery
* Stock management
* Shopping cart
* Checkout with payment simulation
* Wishlist
* User profile
* Order history
* Downloadable / printable invoices

### 🛠️ Admin Dashboard

* Dashboard with KPI statistics
* Data visualization with Chart.js
* Product management
* Category management
* User management
* Order management
* CRUD operations
* Stock management

### 🔔 Real-Time Features

* Real-time order status updates
* Pusher integration for real-time notifications

---

## 🧰 Tech Stack

### Frontend

* **React**
* **Vite**
* **React Router DOM**
* **Context API**
* **Lucide Icons**
* **Chart.js**
* **CSS**

### Backend

* **Node.js**
* **Express.js**
* **MongoDB**
* **Mongoose**

### Real-Time Communication

* **Pusher**

### Development

* **Git**
* **GitHub**
* **npm**
* **Vercel**

---

## 🏗️ Architecture

```text
┌──────────────────────────┐
│       React Frontend     │
│                          │
│  Storefront / Dashboard  │
└────────────┬─────────────┘
             │
             │ REST API
             ▼
┌──────────────────────────┐
│      Express + Node.js   │
│                          │
│    Backend / API Layer   │
└───────┬──────────┬───────┘
        │          │
        ▼          ▼
┌─────────────┐  ┌─────────────┐
│   MongoDB   │  │    Pusher   │
│  Database   │  │ Real-time   │
└─────────────┘  │ notifications│
                 └─────────────┘
```

---

## 📁 Project Structure

```text
mern-ecommerce/
│
├── public/                 # Public frontend assets
│
├── src/                    # React frontend
│   ├── components/         # Reusable UI components
│   ├── pages/              # Application pages
│   ├── context/            # React Context
│   ├── assets/             # Frontend assets
│   └── ...
│
├── server/                 # Node.js / Express backend
│   ├── ...
│   └── ...
│
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
├── .gitignore
└── README.md
```

> The structure may evolve as new features are added.

---

## ⚙️ Requirements

Before running the project locally, make sure you have:

* **Node.js**
* **npm**
* **MongoDB**
* A **Pusher** account if real-time notifications are required

Check your Node.js and npm versions:

```bash
node -v
npm -v
```

---

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/Joseph-Nostra/mern-ecommerce.git
```

### 2. Go to the project directory

```bash
cd mern-ecommerce
```

### 3. Install frontend dependencies

```bash
npm install
```

### 4. Install backend dependencies

```bash
cd server
npm install
```

---

## 🔐 Environment Variables

Create a `.env` file inside the `server/` directory.

Example:

```env
MONGODB_URI=your_mongodb_connection_string

PUSHER_APP_ID=your_pusher_app_id
PUSHER_KEY=your_pusher_key
PUSHER_SECRET=your_pusher_secret
PUSHER_CLUSTER=your_pusher_cluster
```

> Never commit your `.env` file or expose your private credentials.

---

## 💻 Running the Application

### Start the frontend

From the project root:

```bash
npm run dev
```

Vite will start the development server, usually at:

```text
http://localhost:5173
```

### Start the backend

Open another terminal:

```bash
cd server
npm start
```

The backend API will start using the configuration defined in the server environment.

---

## 🏗️ Production Build

To create an optimized frontend production build:

```bash
npm run build
```

To preview the production build locally:

```bash
npm run preview
```

---

## 🌐 Deployment

The project has a production deployment on **Vercel**.

### Live Demo

https://react-sooty-eta.vercel.app/

The frontend is built with Vite and deployed as the production web application.

---

## 🧪 Project Status

**Status:** MVP completed

The current version includes the main customer and admin functionalities required for the MVP.

Future improvements may include:

* Integration with a real payment provider
* Additional security improvements
* More advanced product management
* Additional analytics
* Expanded automated testing
* Further UI/UX improvements

---

## 📌 Important Notes

The checkout currently uses a **payment simulation** and does not process real payments.

The application requires the appropriate MongoDB and Pusher configuration for the backend and real-time functionality.

---

## 👨‍💻 Author

**Youssef Zhar**

GitHub:
https://github.com/Joseph-Nostra

---

## 📄 License

This project is a personal development project created for educational and portfolio purposes.

---
