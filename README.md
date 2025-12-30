# flask-node-docker-app
# Node.js Frontend & Flask Backend using Docker

This project demonstrates a simple microservice-based web application where a **Node.js (Express) frontend** communicates with a **Flask backend**.  
Both services are containerized using **Docker** and connected using **Docker Compose**.

---

## Project Overview

- Frontend built using **Node.js and Express**
- Backend built using **Flask (Python)**
- Frontend sends form data to backend using HTTP POST
- Backend processes the data and returns a JSON response
- Both services run in separate Docker containers
- Docker Compose is used to manage and connect the containers

---

## 📂Folder Structure

flask-node-docker-app/
│
├── frontend/
│ ├── server.js
│ ├── package.json
│ ├── Dockerfile
│ ├── views/
│ │ └── index.ejs
│ └── .gitignore
│
├── backend/
│ ├── app.py
│ ├── requirements.txt
│ ├── Dockerfile
│ └── .gitignore
│
├── docker-compose.yml
└── README.md


---

##  Technologies Used

- **Node.js**
- **Express.js**
- **Flask**
- **Docker**
- **Docker Compose**
- **HTML / EJS**

---

##  How the Application Works

1. User accesses the Node.js frontend in the browser.
2. A form is displayed to the user.
3. On form submission, data is sent to the Flask backend.
4. Flask processes the request and returns a JSON response.
5. The response is displayed to the user.

---

## Docker Setup

- Separate `Dockerfile` for frontend and backend
- Containers communicate using Docker Compose service names
- Both services run on the same Docker network

---

##  How to Run the Project

### Step 1: Build Docker images
```bash
docker-compose build

docker-compose up

http://localhost:3000
docker-compose down
