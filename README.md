# Project Deployment in Docker

This repository contains the Docker Compose files and configurations necessary to deploy the **TypeScript Node.js backend** and **React frontend (built with Vite)** for the [openAgent demo app]. The setup runs both the frontend and backend in Docker containers, with port mapping for easy local development and testing.

## Prerequisites

Ensure that you have the following installed on your machine:

1. **Docker**: [Install Docker](https://docs.docker.com/get-docker/)
2. **Docker Compose**: Docker Compose is bundled with Docker Desktop, so no separate installation is necessary if you have Docker Desktop.

## Project Structure

This repository uses Docker Compose to orchestrate both the backend and frontend services, each pulled from separate GitHub repositories.

- **Backend**: Node.js (TypeScript), served on port `8001`
- **Frontend**: React (Vite), served on port `5173` (mapped to `5001` on the host)

## Getting Started

### Step 1: Clone this Repository

```bash
git clone https://github.com/HongyuYang296/openAgent-deployment.git
cd openAgent-deployment-main
```

### Step 2: Build and Run the Containers
This project uses Docker Compose to manage the frontend and backend services. To build and run the Docker containers, use the following command:

```bash
docker-compose up --build
```
This will do the following:

Build and start the backend service, pulling from the backend repository.
Build and start the frontend service, pulling from the frontend repository and running the Vite development server with access from the host.

### Step 3: Access the Application
Once the containers are running, you can access the services through the following URLs:

Frontend (React with Vite): http://localhost:5001
Backend (Node.js API): http://localhost:8001

