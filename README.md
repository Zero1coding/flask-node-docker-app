# Node.js Frontend and Flask Backend using Docker

This repository contains a simple microservice-based web application where a **Node.js (Express) frontend** communicates with a **Flask backend**.  
Both services are containerized using **Docker** and managed using **Docker Compose**.

---

## Project Overview

- Frontend developed using Node.js and Express
- Backend developed using Flask (Python)
- Frontend sends form data to backend via HTTP POST
- Backend processes data and returns JSON response
- Docker used to containerize both services
- Docker Compose used to run services in the same network

---

## Folder Structure
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

## Technologies Used

- Node.js
- Express.js
- Flask
- Docker
- Docker Compose
- HTML / EJS

---

## How the Application Works

1. User opens the Node.js frontend in a web browser.
2. A form is displayed to the user.
3. On submission, form data is sent to the Flask backend.
4. Flask processes the request and sends a JSON response.
5. The response is returned to the frontend.

---
## Run Instructions

```yaml
run_instructions:
  prerequisites:
    - Docker installed and running
    - Docker Compose available

  steps:
    - Navigate to project root directory
      command: cd flask-node-docker-app

    - Build Docker images
      command: docker-compose build

    - Start containers
      command: docker-compose up

    - Access application
      url: http://localhost:3000

    - Stop containers
      command: docker-compose down
---
## Screenshots
## Application Running
<img width="1911" height="1018" alt="Application Running" src="https://github.com/user-attachments/assets/3a9ed849-b442-42f8-8850-5bf930f3cebc" />
## Docker Containers
<img width="804" height="289" alt="Docker Containers" src="https://github.com/user-attachments/assets/d22ddf88-496f-434e-8286-139edde246c9" />
## Docker Images
<img width="735" height="261" alt="Docker Images" src="https://github.com/user-attachments/assets/9396cf4d-97bb-49f7-b54f-4298b812f50a" />
## Docker Compose Execution
<img width="1919" height="1017" alt="Docker Compose Execution" src="https://github.com/user-attachments/assets/bcec6873-aa90-4e45-accb-517360a1772f" /> ```
