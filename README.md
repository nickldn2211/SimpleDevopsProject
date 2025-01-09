# DevOps Project: Build Jenkins CI/CD Pipeline for Simple Web Application


![project](https://github.com/user-attachments/assets/cd825ee2-c3ba-47c0-905b-e83c8a2857e0)

## Tech Stack
- **Containerization**: Docker
- **Vulnerability scanning**: Trivy
- **CI/CD service**: Jenkins
- **Version control and collaboration**: GitHub
- **Cloud service**: AWS EC2

## Pipeline Stages

1. **Clean Workspace**: Clears the workspace to ensure a clean environment.
2. **Clone GitHub Repository**: Clones the specified branch of the GitHub repository.
3. **Build Docker Image**: Uses the Dockerfile to build a Docker image.
4. **Run Unit Tests**: Executes unit tests using Maven to ensure code quality.
5. **Security Scan**: Runs a security scan on the Docker image using Trivy.
6. **Push Docker Image**: Pushes the Docker image to Docker Hub.
7. **Deploy Application**: Pulls down the Docker image from Docker Hub and runs the web application locally.
8. **Post-Deployment Health Check**: Verifies the application is running.
#### Post Actions
- **Success**: Echoes a message indicating the pipeline completed successfully.
- **Failure**: Echoes a message indicating the pipeline failed.
