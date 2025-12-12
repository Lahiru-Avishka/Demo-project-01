📦 Docker + Nginx Demo Project

This is a simple demo project that shows how to deploy a static website using Docker and Nginx.
The application files are served through Nginx using a custom Dockerfile, making the setup lightweight, fast, and easy to deploy.

🚀 Features

Serves static HTML/CSS/JS using Nginx

Custom Dockerfile for easy deployment

Lightweight container-based setup

Fast local development and testing

📁 Project Structure
.
├── Dockerfile
├── index.html
├── styles.css
└── (other static assets)

🛠️ Dockerfile
FROM nginx:latest
ADD . /usr/share/nginx/html

▶️ How to Run
1. Build the Docker image
docker build -tag nginx-demo .

2. Run the container
docker run -d -p 8081:80 nginx-demo

3. Open in browser

Visit:

http://localhost:8085

📦 Stop & Remove Container
docker ps
docker stop <container_id>
docker rm <container_id>

📝 Description

This project demonstrates how to deploy a static web application using Docker and Nginx.
It is useful for learning containerisation, exploring web server deployment, and testing simple frontend projects inside a real server environment.