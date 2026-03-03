📝 Todo List

   A full-stack Todo List app where you can add tasks, mark them as completed or pending, filter, search, and paginate them.



🛠️ Tech Stack

  •	Frontend: React, Axios, Material UI
  •	Backend: Node.js, Express
  •	Database: MongoDB, Mongoose


📁 Project Structure

```
todo_list_task/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── package.json
│
├── backend/
│   ├── models/
│   │   └── Task.js
│   ├── routes/
│   │   └── tasks.js
│   ├── server.js
│   └── package.json
│
└── README.md
```

⚙️ How to Run

1. Clone the Repository

  •	bash
  •	git clone https://github.com/OptimityLogics/Todo-Task
  •	cd todo_list_task

2. Backend

  •	bash
  •	cd backend
  •	npm install
  •	npm run dev

3. Frontend

  •	bash
  •	cd frontend
  •	npm install
  •	npm run dev
  •	Open `http://localhost:5173` in your browser.
  •	Make sure MongoDB is running locally before starting the backend.


📡 API Endpoints

| Method | Endpoint              | Description                                                        |
|--------|-----------------------|--------------------------------------------------------------------|
| GET    | `/tasks/all`          | Fetch all tasks (supports `page`, `limit`, `search` query params)  |
| POST   | `/tasks/create`       | Create a new task                                                  |
| PUT    | `/tasks/update/:id`   | Toggle task status (completed ↔ pending)                           |
| GET    | `/tasks/all/:status`  | Filter tasks by `completed` or `pending`                           |


