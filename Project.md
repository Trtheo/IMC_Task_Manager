# ERD & Relationships
## Entities:

### User

- _id (ObjectId)

- email (String, unique)

- password (String)

- tasks (Array of Task refs)

### Task

- _id (ObjectId)

- title (String)

- description (String)

- priority (String: "High"/"Medium"/"Low")

- status (String: "Pending"/"Completed")

- user (ObjectId ref to User)

### Relationship:
- User → (1-to-Many) → Task

## Project Structure

```bash
task-manager/
├── backend/
│   ├── node_modules/
│   ├── models/
│   │   ├── User.js
│   │   └── Task.js
│   ├── routes/
│   │   ├── auth.js
│   │   └── tasks.js
│   ├── controllers/
│   │   ├── authController.js
│   │   └── taskController.js
│   ├── middleware/
│   │   └── auth.js
│   ├── .env
│   ├── package.json
│   └── server.js
└── frontend/
    ├── node_modules/
    ├── public/
    ├── src/
    │   ├── components/
    │   │   ├── TaskList.jsx
    │   │   ├── AddTask.jsx
    │   │   ├── Login.jsx
    │   │   └── Register.jsx
    │   ├── context/
    │   │   ├── AuthContext.jsx
    │   │   └── TaskContext.jsx
    │   ├── services/
    │   │   └── api.js
    │   ├── App.jsx
    │   └── index.js
    ├── package.json
    └── tailwind.config.js
```