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

Getting Started

Follow these steps to set up and run the project:

Clone the repository
```bash
git clone https://github.com/pritibhosale20/3-Tier-Architecture_Docker-Compose.git
cd 3-Tier-Architecture_Docker-Compose
```
Start the containers
```
docker-compose up -d
```
Access the application

Open your browser and go to: http://localhost

Stop the containers (when finished)

```docker-compose down```
     
# Components
frontend/ → Contains Nginx configuration and static files.

backend/ → Contains PHP application logic and Dockerfile.

database/ → Contains SQL initialization scripts.

docker-compose.yml → Defines the services and networking.
