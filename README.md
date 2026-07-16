# 🚀 Dockerized Python Application with Nginx Load Balancer

## 📖 Project Overview

This project demonstrates how to deploy a Python Flask application using **Docker** and **Docker Compose**, with **Nginx** configured as a reverse proxy and load balancer. Three backend containers run the same Flask application, while Nginx distributes incoming client requests among them using the **Round Robin** load-balancing algorithm. This setup improves application availability, scalability, and traffic distribution.

---

## 🛠️ Technologies Used

- Docker
- Docker Compose
- Python (Flask)
- Nginx
- Linux

---

## 📂 Project Structure

```text
.
├── Dockerfile
├── docker-compose.yml
├── nginx.conf
├── app.py
├── requirements.txt
└── README.md
```

---

## 🚀 Steps to Run the Project


### Step 2: Build Docker Images and Start Containers

```bash
docker compose up -d --build
```

### Step 3: Verify Running Containers

```bash
docker ps
```

### Step 4: Open the Application

Open your browser and visit:

```text
http://<EC2-Public-IP>
```

### Step 5: Verify Load Balancing

Refresh the browser several times. Nginx distributes requests across the backend containers, and you'll see different container hostnames, for example:

```text
Hello from backend-1!
Hello from backend-2!
Hello from backend-3!
```

### Step 6: Stop the Project

```bash
docker compose down
```

---

## 🎯 Learning Outcomes

- Built Docker images for a Python Flask application.
- Managed multiple containers using Docker Compose.
- Configured Nginx as a reverse proxy and load balancer.
- Implemented Round Robin load balancing.
- Understood Docker networking and inter-container communication.
- Deployed a scalable multi-container application.

---

## 👨‍💻 Author

**Charan Vardhan Katta**
