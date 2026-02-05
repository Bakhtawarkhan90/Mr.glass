Mr. Glass – Static Website (Dockerized)

A clean and responsive static website built using HTML, CSS, and JavaScript, containerized with Docker and served using Nginx.

Project Overview
Type: Static Website
Frontend: HTML, CSS, JavaScript
Web Server: Nginx
Containerization: Docker
Deployment Ready: EC2 / VPS / On-Prem Linux Server

Project Structure
Mr.glass/
index.html
about.html
work.html
thankyou.html
style.css
script.js
images/
pdfs/
Dockerfile

Getting Started

Prerequisites
Ubuntu / Linux system
Internet connection
Sudo access

Docker Installation
sudo apt update
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
docker --version

Docker User Permission
sudo usermod -aG docker $USER
newgrp docker

Build Docker Image
cd Mr.glass
docker build -t mr-glass-website .

Run the Container
docker run -d -p 80:80 --name mr-glass mr-glass-website

Access the Website
http://localhost
or
http://<server-ip>

Stop and Remove Container
docker stop mr-glass
docker rm mr-glass
docker rmi mr-glass-website

Architecture Decisions
Docker for consistency
Nginx for performance
Static design for simplicity

Author
Bakhtawar Khan



. ## Home Page
![glass](./glass.png)
