# node-todo-cicd

Run these commands:


`sudo apt install nodejs`


`sudo apt install npm`


`npm install`

`node app.js`

or Run by docker compose

test


# 🚀 Node.js DevOps CI/CD Pipeline on AWS

## 📌 Project Overview

This project demonstrates an end-to-end DevOps CI/CD pipeline by deploying a Node.js application on an AWS EC2 instance using GitHub, Jenkins, Docker, and GitHub Webhooks. The pipeline automatically detects code changes, builds a Docker image, and deploys the latest version of the application inside a Docker container without manual intervention.

## 🛠️ Technologies Used

* AWS EC2 (Ubuntu)
* Linux
* Git & GitHub
* GitHub Webhooks
* Jenkins
* Docker
* Node.js
* Shell Scripting

## 📂 CI/CD Workflow

1. Developer pushes code to the GitHub repository.
2. GitHub Webhook sends an HTTP POST request to Jenkins.
3. Jenkins automatically triggers the pipeline.
4. Jenkins pulls the latest source code from GitHub.
5. Jenkins builds a new Docker image.
6. The existing Docker container is stopped and removed (if present).
7. A new Docker container is created using the latest Docker image.
8. The updated application is deployed and becomes accessible through the AWS EC2 Public IP.

## 🔔 GitHub Webhooks

GitHub Webhooks were configured to automate the CI/CD process.

* Configured a webhook in the GitHub repository pointing to the Jenkins webhook endpoint.
* Enabled automatic build triggering on every code push.
* Eliminated the need for manually starting Jenkins builds.
* Achieved continuous integration by automatically validating and deploying every new commit.

## 📁 Project Structure

```text
node-todo-app/
├── Dockerfile
├── Jenkinsfile
├── package.json
├── server.js
├── README.md
└── ss/
    ├── architecture.png
    ├── github-webhook.png
    ├── jenkins-dashboard.png
    ├── jenkins-success.png
    ├── docker-images.png
    ├── docker-container.png
    └── application.png
```

## ⚙️ Features

* Automated CI/CD using Jenkins
* GitHub Webhook integration
* Docker containerization
* AWS EC2 deployment
* Automated application deployment after every GitHub push
* Linux-based server management
* Zero manual deployment after code commits

## 📸 Project Screenshots

### GitHub Webhook Configuration

![GitHub Webhook](ss/21.png)

### Jenkins Dashboard

![Jenkins Dashboard](ss/jenkins-dashboard.png)

### Successful Jenkins Pipeline

![Jenkins Pipeline](ss/jenkins-success.png)

### Docker Images

![Docker Images](ss/docker-images.png)

### Running Docker Container

![Docker Container](ss/docker-container.png)

### Application Running on AWS EC2

![Application](ss/application.png)

## 🎯 Learning Outcomes

* Configured GitHub Webhooks to trigger Jenkins automatically.
* Built an automated CI/CD pipeline using Jenkins.
* Containerized a Node.js application using Docker.
* Deployed applications on AWS EC2.
* Integrated GitHub, Jenkins, Docker, and AWS into a complete deployment workflow.
* Practiced Linux administration, Git, Docker, and CI/CD automation.

## 👨‍💻 Author

**Sarthak Kumar**

