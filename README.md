# Three Tier Architecture using Docker-compose
This repository demonstrates a simple three-tier architecture using Docker Compose. The architecture consists of the following tiers:

# Architecture Overview
Frontend (Web Tier)
Uses Nginx as a web server to serve static content (HTML, CSS, JavaScript) and act as a reverse proxy to the backend.

Backend (App Tier)
A PHP-based application that handles dynamic requests and business logic.

Database (Data Tier)
A MySQL database used for persistent data storage.

# Prerequisites
Ensure you have the following installed on your system before running this project:
1. Docker 
2. Docker Compose 

# Repository Structure
📂 ThreeTierArchitecture

├── 📂 apptier

     ├── Dockerfile
     ├── 📂 myphpcode
          ├── index.php
          
├── 📂 dbtier
     ├── Dockerfile
     ├── init.sh
     ├── init.sql  
     
├── 📂 webtier
     ├── Dockerfile
     ├── default.conf
     ├── 📂 myhtmlcode
          ├── index.html  
          
├── docker-compose.yml          
     
# Components
frontend/ → Contains Nginx configuration and static files.
backend/ → Contains PHP application logic and Dockerfile.
database/ → Contains SQL initialization scripts.
docker-compose.yml → Defines the services and networking.
