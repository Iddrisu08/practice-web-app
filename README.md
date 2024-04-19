# Practice-web-app

This repository contains a simple web applications that can be built and deployed using Docker. It also includes configuration files for Jenkins automation.

## Prerequisites

- Java Development Kit (JDK) installed on your machine.
- Docker installed and running on your machine.
- (Optional) Jenkins server for automated builds and deployments.

## Build and Run with Docker

### 1. Build Docker Image

To build the Docker image of the web applications, navigate to the project directory and run:

```
docker build -t your-image-name:image-tag .
```

### 2. Run Docker Container
After building the Docker image, start a Docker container from the image:

```
docker run -d --name image/container:tag -p system-port:container-port image-name
```
Access the running web application at `http://localhost:system-port` in your web browser.

## Jenkins Automation
This repository includes a `Jenkinsfile` for automating the build and deployment process using Jenkins. Configure a Jenkins pipeline to execute the `Jenkinsfile` for continuous integration and continuous deployment (CI/CD).

