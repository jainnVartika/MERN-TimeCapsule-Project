# Time Capsule- A MERN website

A full-stack MERN (MongoDB, Express, React, Node.js) application for creating, viewing, and managing memories. Users can add posts with titles, messages, and images. This project demonstrates a complete MERN stack workflow with a React frontend and Node/Express backend.

---

## **Project Structure**

project_mern_memories-PART_1_and_2/
│
├── client/ # React frontend
│ ├── public/
│ ├── src/
│ ├── package.json
│ └── ...
│
├── server/ # Node.js + Express backend
│ ├── models/ # Mongoose models
│ ├── routes/ # API routes
│ ├── index.js # Main server file
│ ├── package.json
│ └── ...
│
├── .gitignore
├── README.md
└── ...

yaml
Copy code

---

## **Features**

- Add new posts (title, message, optional image)
- View all posts
- Responsive UI
- Full CRUD operations possible (extendable)
- MongoDB integration for data storage
- API routes protected with CORS support

---

## **Technologies Used**

- **Frontend:** React, Axios, React Router, CSS/Material UI (optional)
- **Backend:** Node.js, Express.js
- **Database:** MongoDB with Mongoose
- **Other:** CORS, dotenv for environment variables

---

## **Installation**

### **Prerequisites**

- Node.js (v16 recommended)
- npm
- MongoDB (local or Atlas)

### **Setup Backend**

```bash
cd server
npm install
# Create a .env file with your MongoDB URI
# Example:
# MONGO_URI=your_mongodb_connection_string
npm start
Server runs on http://localhost:5000 by default.

Setup Frontend
bash
Copy code
cd client
npm install
npm start
Frontend  http://localhost:3000 (CRA).

Environment Variables
Create .env files in server/ and client/ if needed:

server/.env

ini
Copy code
MONGO_URI=your_mongodb_connection_string
PORT=5000
client/.env (optional)

ini
Copy code
REACT_APP_API_URL=http://localhost:5000
API Endpoints
GET /posts – Get all posts

POST /posts – Create a new post

GET /posts/:id – Get a single post

PATCH /posts/:id – Update a post

DELETE /posts/:id – Delete a post

Usage
Start the backend server.

Start the frontend.

Open the browser at http://localhost:5173 (or 3000).

Add and view memories in the UI.

Deployment
This project can be deployed using platforms like:

Frontend: Vercel, Netlify

Backend: Render, Railway, Heroku

Tip: Make sure to update the frontend API URL to the live backend URL when deploying.

Contributing
Fork the repository

Create your branch (git checkout -b feature-name)

Commit your changes (git commit -m 'Add feature')

Push to branch (git push origin feature-name)

Create a pull request