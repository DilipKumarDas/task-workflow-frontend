# TaskFlow Frontend

TaskFlow Frontend is a React-based user interface for the TaskFlow application.  
It connects with the backend REST API to create, search, update, and manage tasks.

---
Features

- Add new tasks  
- View all tasks  
- Update task status  
- Search tasks by title  
- Clean, centered UI layout  
- Fully responsive  
- Integrated with the TaskFlow backend  

---

Tech Stack

- React (Vite)
- JavaScript
- Axios
- CSS
- Vercel Deployment

---

Project Structure

taskflow-frontend/
├── src/
│ ├── components/
│ │ ├── TaskForm.jsx
│ │ ├── TaskList.jsx
│ │ ├── SearchBar.jsx
│ │ └── api.js
│ ├── App.jsx
│ └── main.jsx
├── public/
├── package.json
└── vite.config.js


---
Running Locally

1. Clone the repository
```bash
git clone https://github.com/DilipKumarDas/taskflow-frontend.git
cd taskflow-frontend

2. Install dependencies

npm install

3. Start development server

npm run dev

Frontend will be available at:

http://localhost:5173

🔌 Backend Integration

Update your backend API base URL inside:

src/components/api.js

Example:

import axios from "axios";

export default axios.create({
  baseURL: "https://taskflow-backend.onrender.com"
});

🐳 Build for Production

npm run build

Production files will be generated in:

dist/

☁️ Deployment

You can deploy using:
Vercel

    Create a new Vercel project

    Select this repo

    Set build command:

npm run build

Output directory:

    dist


Edit api.js:

export default axios.create({
  baseURL: import.meta.env.VITE_API_URL
});
