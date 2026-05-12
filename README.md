# 🚀 CodeAlpha - Web Server using Docker (Task 4)

## 📌 Overview
This project is part of the CodeAlpha DevOps Internship.  
It demonstrates how to deploy and manage a simple web server using Docker and Nginx.

The goal of this task is to understand Docker containerization, port mapping, and volume mounting in real-world usage.

---

## 🛠 Technologies Used
- Docker
- Nginx
- HTML

---

## 📁 Project Structure

CodeAlpha_WebServer_Docker/
│
├── test.html
└── README.md

---

## ⚙️ How It Works
In this project, an Nginx container is used to serve a custom HTML file.

The HTML file is mounted from the local machine into the container using a Docker volume.  
This allows any changes made to the file on the host machine to be reflected immediately inside the container.

---

## 🚀 Run Instructions

### ▶️ Start the container
🌐 Access the Web Server

After running the container, open your browser and visit:

http://localhost:8080

You will see the custom HTML page served by Nginx.

📌 Key Concepts Learned
Docker container lifecycle (run, stop, remove)
Port mapping using -p
Volume mounting using -v
Running Nginx inside Docker
Serving static websites using containers
🧪 Docker Commands Used
# Run container
docker run -d -p 8080:80 --name webserver -v "C:\Users\user\Downloads\CodeAlpha_WebServer_Docker\test.html:/usr/share/nginx/html/index.html" nginx

# Check running containers
docker ps

# View logs
docker logs webserver

# Stop container
docker stop webserver

# Remove container
docker rm webserver
🧠 Learning Outcome

By completing this task, I learned how to:

Deploy a web server using Docker
Use Nginx inside a container
Connect local files to containers using volumes
Manage container lifecycle using Docker CLI
Understand basic DevOps containerization workflow
📸 Screenshots (To Be Added)
Docker container running (docker ps)
Web page output (localhost:8080)
Docker logs output
Image list (docker images)
👨‍💻 Author

Abdelaziz Hassan
DevOps Internship - CodeAlpha

```bash
docker run -d -p 8080:80 --name webserver -v "C:\Users\user\Downloads\CodeAlpha_WebServer_Docker\test.html:/usr/share/nginx/html/index.html" nginx
