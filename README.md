# 📝 Todo List App

A full-stack Todo List app where you can add tasks, mark them as completed or pending, filter, search, and paginate them.

---

## 🛠️ Tech Stack

- **Frontend:** React, Axios, Material UI
- **Backend:** Node.js, Express
- **Database:** MongoDB, Mongoose

---

## 📁 Project Structure

```
Todo-Task/
├── backend/
│   ├── src/
│   │   ├── common/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── middlewares/
│   │   ├── models/
│   │   ├── routes/
│   │   └── validation/
│   ├── app.js
│   ├── server.js
│   ├── .env
│   └── package.json
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── api/
│   │   ├── assets/
│   │   ├── App.css
│   │   ├── App.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   ├── .gitignore
│   ├── eslint.config.js
│   ├── index.html
│   └── package.json
│
├── .gitignore
└── README.md
```

---

## ⚙️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/OptimityLogics/Todo-Task
cd Todo-Task
```

### 2. Backend

```bash
cd backend
npm install
npm run dev
```

### 3. Frontend

```bash
cd frontend
npm install
npm run dev
```

Open `http://localhost:5173` in your browser.

> Make sure MongoDB is running locally before starting the backend.

---

## 📡 API Endpoints

| Method | Endpoint              | Description                              |
|--------|-----------------------|------------------------------------------|
| GET    | `/tasks/all`          | Fetch all tasks (supports `page`, `limit`, `search` query params) |
| POST   | `/tasks/create`       | Create a new task                        |
| PUT    | `/tasks/update/:id`   | Toggle task status (completed ↔ pending) |
| GET    | `/tasks/all/:status`  | Filter tasks by `completed` or `pending` |

---

## ✨ Features

- Add new tasks
- Toggle task status using a checkbox
- Filter tasks — All, Completed, Pending
- 🔍 Search tasks by title
- 📄 Pagination to browse tasks page by page
- Frontend syncs with backend on every action
