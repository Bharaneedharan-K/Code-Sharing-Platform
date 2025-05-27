# 🚀 Code Snippet Sharing Platform

A full-stack web application that allows developers to create, share, like, and comment on code snippets. Built using the MERN stack (MongoDB, Express, React, Node.js) with secure JWT-based authentication.

## 🌐 Live Demo

- **Frontend (Vercel)**: [https://binfn.vercel.app](https://binfn.vercel.app)
- **Backend (Render)**: [https://binfn.onrender.com](https://https://binfn.onrender.com)

---

## 📸 Features

### 🔐 Authentication
- User registration and login using JWT

### 🧠 Snippet Management
- Create, read, update, and delete code snippets
- Fields include title, description, language, tags, and the code itself
- Search snippets by keyword or user

### ❤️ Interactions
- Like or unlike any snippet
- Add comments with timestamps
- View snippet details including likes and comments

---

## 🛠 Tech Stack

### 🔧 Backend
- Node.js
- Express.js
- MongoDB & Mongoose
- JWT for authentication
- Helmet, CORS for security and logging

### 🎨 Frontend
- React (with Hooks)
- Axios for API communication
- Tailwind CSS for styling

### ☁ Hosting
- **Frontend**: Vercel
- **Backend**: Render

---

## 🚀 Getting Started Locally

### Backend

1. Clone the repository:
   ```bash
   git clone https://github.com/Bharaneedharan-K/Code-Sharing-Platform.git
   cd server
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file:
   ```
   PORT= your_port_number
   MONGODB_URI=your_mongodb_connection
   ACCESS_TOKEN_SECRET=your_jwt_secret
   ```

4. Start the server:
   ```bash
   npm start
   ```

### Frontend

1. Navigate to the frontend directory:
   ```bash
   cd ../client
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the frontend:
   ```bash
   npm start
   ```

---

## 📡 API Overview

### Auth Routes

| Method | Endpoint        | Description       |
|--------|------------------|-------------------|
| POST   | /api/auth/signup | Register new user |
| POST   | /api/auth/login  | Login and get JWT |

### Snippet Routes

| Method | Endpoint            | Description                |
|--------|---------------------|----------------------------|
| POST   | /api/snippets       | Create a snippet           |
| GET    | /api/snippets       | Get all snippets           |
| GET    | /api/snippets/:id   | Get snippet by ID          |
| PUT    | /api/snippets/:id   | Update snippet             |
| DELETE | /api/snippets/:id   | Delete snippet             |

### Like and Comment Routes

| Method | Endpoint                        | Description                |
|--------|----------------------------------|----------------------------|
| PATCH  | /api/snippets/:id/like          | Like or unlike a snippet   |
| POST   | /api/snippets/:id/comment       | Add a comment              |
| GET    | /api/snippets/:id/comments      | Get comments for snippet   |

---

## 🧠 License

This project is licensed under the [MIT License](LICENSE).
