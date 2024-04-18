# Practice-web-app

This repository contains a simple Maven-generated web application that can be built and deployed using Docker. It also includes configuration files for Jenkins automation.

## Project Structure

- **`src/`**: Contains the source code for the web application.
- **`pom.xml`**: Maven project configuration file.
- **`Dockerfile`**: Dockerfile for building a Docker image of the web application.
- **`Jenkinsfile`**: Jenkins pipeline script for CI/CD automation.

## Prerequisites

- Java Development Kit (JDK) installed on your machine.
- Docker installed and running on your machine.
- (Optional) Jenkins server for automated builds and deployments.

## Build and Run with Docker

### 1. Build Docker Image

To build the Docker image of the web application, navigate to the project directory and run:

```
docker build -t practice-web-app:v1 .
```

### 2. Run Docker Container
After building the Docker image, start a Docker container from the image:

```
docker run -d --name practice-web-app -p 8080:8080 practice-web-app
```
Access the running web application at `http://localhost:8080` in your web browser.

## Jenkins Automation
This repository includes a `Jenkinsfile` for automating the build and deployment process using Jenkins. Configure a Jenkins pipeline to execute the Jenkinsfile for continuous integration and continuous deployment (CI/CD).

