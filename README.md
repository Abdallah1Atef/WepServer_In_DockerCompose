# DockServe: Web Server in Docker Compose

## Overview
**DockServe** is a project that demonstrates how to set up a **web server** using **Docker Compose**. It provides a simple and scalable way to deploy a web application in a containerized environment. The project includes a basic web server (e.g., Nginx or Apache) and demonstrates how to manage multi-container applications using Docker Compose.

---

## Features
- **Containerized Web Server**: Deploy a web server (e.g., Nginx or Apache) inside a Docker container.
- **Docker Compose**: Use Docker Compose to define and manage multi-container applications.
- **Scalability**: Easily scale the web server by modifying the Docker Compose configuration.
- **Portability**: The entire setup is portable and can be run on any system with Docker installed.

---

## How It Works

### 1. **Dockerfile**
The `Dockerfile` defines the environment for the web server. For example:
```Dockerfile
FROM nginx:alpine
COPY index.html /usr/share/nginx/html
"index.php" file contains the code for the home web page. "db.php" file contains the code for the page where the data is shown from the database. "db" folder contains the script for the database creation in "MySQL". In order to use the files, first, you have to build an 'image' using the dockerfile called "project", second, use the docker-compose file to run the server and connect the containers together, last thing, go on your browser and type in the URL 'localhost:80/index.php', and with these steps you should be able to see our work :).
