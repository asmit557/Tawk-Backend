# 💬 Chat App Backend – Real-Time Conversations with Socket.IO & ZEGOCLOUD ⚡

> Scalable and secure backend for a real-time chat application. Built with **Express.js**, integrated with **Socket.IO** for live messaging, and powered by **ZEGOCLOUD** for voice/video communication.

---

## 🌐 Frontend Repository

👉 [Chat App Frontend (React)](https://github.com/asmit557/Tawk-React-Chat-App-)

---

## 🛠️ Tech Stack

* 🖥️ **Node.js + Express.js**
* 🧱 **MongoDB + Mongoose**
* 🧩 **Socket.IO** – Real-time bidirectional event-based communication
* 📡 **ZEGOCLOUD** – Audio & video conferencing
* 🔐 **JWT Auth + bcryptjs** for authentication
* 🧼 **Security Middlewares**: Helmet, xss-clean, express-rate-limit, mongo-sanitize
* 📧 **SendGrid** for email services

---

## 🔐 Features

* ✅ **JWT Authentication**
* 🔒 **Secure Password Hashing** with bcryptjs
* 🛡️ **Rate Limiting, XSS, & NoSQL Injection Protection**
* 🧼 **Cookie Sessions & Parser**
* 📩 **OTP Verification** (otp-generator)
* 📨 **Email Service** via SendGrid
* 🧭 **Cross-Origin Access** with CORS
* 📊 **Logging Middleware** with Morgan
* 🔌 **Real-Time Messaging** with Socket.IO
* 🎥 **ZEGOCLOUD Integration** (Frontend uses SDK for video/audio calls)

---

## 🚀 Getting Started

### 🔧 Prerequisites

* Node.js v18+
* MongoDB instance
* ZEGOCLOUD account
* SendGrid API key

### 📦 Clone the Repository

```bash
git clone https://github.com/asmit557/Tawk-Backend.git
cd Tawk-Backend
```

### 🛠️ Install Dependencies

```bash
npm install
```

### 📁 Set Up Environment Variables

Create a `.env` file in the root with the following:

```env
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
SENDGRID_API_KEY=your_sendgrid_key
CLIENT_URL=http://localhost:3000
```

### 🏁 Start the Server (Dev Mode)

```bash
npm start
```

> Make sure MongoDB is running and `.env` is properly configured.

---

## 🧪 API Endpoints (Summary)

| Method | Endpoint               | Description                  |
| ------ | ---------------------- | ---------------------------- |
| POST   | /api/auth/register     | Register a new user          |
| POST   | /api/auth/login        | Login with credentials       |
| GET    | /api/users/me          | Get current user info        |
| POST   | /api/otp/verify        | OTP verification endpoint    |
| GET    | /api/messages/\:roomId | Get messages for a chat room |

More detailed documentation coming soon...

---

## 📚 Notable Packages

| Package                | Use Case                             |
| ---------------------- | ------------------------------------ |
| **socket.io**          | Real-time messaging engine           |
| **mongoose**           | MongoDB object modeling              |
| **helmet**             | Secures Express apps                 |
| **xss-clean**          | Prevent XSS attacks                  |
| **express-rate-limit** | Limit API usage to avoid brute force |
| **cookie-session**     | Lightweight session store            |
| **@sendgrid/mail**     | Email sending                        |
| **dotenv**             | Environment config                   |
| **cors**               | Enable cross-origin access           |

---

## 👥 Contributing

We welcome pull requests and feedback! Feel free to fork this repo and submit PRs.

---

## 📄 License

This project is licensed under the **ISC License**.

---

## 🙌 Acknowledgements

Special thanks to:

* [Socket.IO](https://socket.io)
* [ZEGOCLOUD](https://www.zegocloud.com)
* [MongoDB](https://www.mongodb.com)
* [SendGrid](https://sendgrid.com)

---

## 🌟 Support the Project

If you like this project, please consider starring it:

[![GitHub Stars](https://img.shields.io/github/stars/asmit557/Tawk-Backend?style=social)](https://github.com/asmit557/Tawk-Backend)

---

Made with ❤️ by [Asmit Verma](https://github.com/asmit557)
