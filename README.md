# 📡 Chat App Backend – Real-time Messaging Engine

![Socket.IO](https://img.shields.io/badge/Socket.io-RealTime-blue?logo=socket.io)
![ZEGOCLOUD](https://img.shields.io/badge/ZEGOCLOUD-Voice%2FVideo%20SDK-blueviolet)
![Express](https://img.shields.io/badge/Express.js-Backend-lightgrey)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-green)

> ⚡ Powering the backend of a modern **React + Socket.IO** chat application with **ZEGOCLOUD** integration for voice and video calling, strong authentication, real-time messaging, and robust security layers.

---

## 📦 Tech Stack

* 🚀 **Express.js** for routing & middleware
* 🗃️ **MongoDB + Mongoose** for database management
* 🔐 **JWT Authentication** with cookie-based session
* 📲 **Socket.IO** for WebSocket communication
* 🎥 **ZEGOCLOUD** for real-time video/audio calls
* 📤 **SendGrid** for email functionality (OTP, verification)
* 🔐 Security middleware: **Helmet**, **XSS-Clean**, **MongoSanitize**, **RateLimiter**

---

## 🗂️ Project Structure

```
chat-app-backend/
├── controllers/
├── models/
├── routes/
├── utils/
├── server.js
├── .env
└── package.json
```

---

## 🚀 Installation & Setup

### 🔧 Prerequisites

* Node.js v16+
* MongoDB instance (local/cloud)
* ZEGOCLOUD App ID & Server Secret
* SendGrid API Key

### 🧬 Clone the Repository

```bash
git clone https://github.com/asmit557/Tawk-Backend.git
cd Tawk-Backend
```

### 📥 Install Dependencies

```bash
npm install
```

### ⚙️ Environment Variables

Create a `.env` file in the root:

```env
PORT=5000
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_jwt_secret
ZEGOCLOUD_APP_ID=your_app_id
ZEGOCLOUD_SERVER_SECRET=your_server_secret
SENDGRID_API_KEY=your_sendgrid_key
```

---

## 💻 Start the Server

```bash
npm start
```

> Starts in development mode using `nodemon` (defined in `start` script)

---

## 🔐 Features

### 👥 Authentication

* JWT token generation & verification
* Cookie-based session management
* OTP verification via SendGrid
* Password hashing with bcrypt

### 💬 Real-Time Messaging

* WebSocket events using Socket.IO
* User online/offline tracking
* Room creation and message broadcasting

### 📹 ZEGOCLOUD Integration

* Voice & video call room support
* Token generation and verification with AppID & secret

### 🛡️ Security Middleware

* `helmet`: Sets security headers
* `xss-clean`: Prevents cross-site scripting
* `express-rate-limit`: Rate limiting on sensitive routes
* `express-mongo-sanitize`: NoSQL injection prevention

---

## 🧪 Development Scripts

| Script      | Description                             |
| ----------- | --------------------------------------- |
| `npm start` | Run backend in dev mode using `nodemon` |

---

## 🧰 Notable Packages

| Package                  | Purpose                                |
| ------------------------ | -------------------------------------- |
| `socket.io`              | Real-time bi-directional communication |
| `bcryptjs`               | Password hashing                       |
| `jsonwebtoken`           | Auth token generation & validation     |
| `express-mongo-sanitize` | Prevent Mongo injection                |
| `helmet`                 | Adds security headers                  |
| `xss-clean`              | XSS protection                         |
| `express-rate-limit`     | Rate limiting                          |
| `@sendgrid/mail`         | Email delivery                         |
| `dotenv`                 | Environment variables                  |

---

## 🛠️ Upcoming Features

* [ ] Message deletion/edit support
* [ ] Group chat support with admins
* [ ] ZEGOCLOUD call history logging
* [ ] Admin dashboard

---

## 📜 License

Licensed under the ISC License. © 2024 Asmit Verma

---

Made with 💬 and ⚡ by [Asmit Verma](https://github.com/asmit557)
