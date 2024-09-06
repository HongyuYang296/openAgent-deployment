# Project Deployment Configuration

This repository contains the Docker Compose files and associated configurations necessary to deploy the TypeScript Node.js backend and React frontend for [Project Name]. This setup is intended to streamline the process of deploying both components in a consistent, reproducible manner.

## Getting Started

These instructions will cover usage information and for the docker container 

### Prerequisites

In order to run this container you'll need docker installed.

* [Windows](https://docs.docker.com/desktop/install/windows-install/)
* [OS X](https://docs.docker.com/desktop/install/mac-install/)
* [Linux](https://docs.docker.com/desktop/install/linux-install/)

### Usage

#### Environment Variables

To modify the environment variables, edit the `.env` file in the root of this repository and adjust the variables as necessary.

- `NODE_ENV` - Specifies the environment in which the backend and frontend are running (development, production, etc.).

#### Building and Running with Docker Compose

To start the entire stack (backend and frontend) with Docker Compose, use the following commands:

```bash
docker-compose up --build
