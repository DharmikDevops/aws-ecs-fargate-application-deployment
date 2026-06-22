# 🚀 AWS ECS Fargate Application Deployment

## 📖 Project Overview

This project demonstrates how to deploy a containerized web application on AWS using Amazon Elastic Container Registry (ECR) and Amazon Elastic Container Service (ECS) with AWS Fargate.

The application was containerized using Docker, stored in Amazon ECR, and deployed as an ECS Fargate task behind an Application Load Balancer (ALB). A new version of the application was created, pushed to ECR, and deployed through ECS to demonstrate container image versioning and application updates.

This project provides hands-on experience with containerization, image repositories, serverless container orchestration, and application deployment on AWS.

---

## 🏗️ Architecture Diagram

![Architecture Diagram](screenshots/architecture-diagram.png)

---

## 🔄 Application Flow

1. User sends an HTTP request through a web browser.
2. Application Load Balancer (ALB) receives the request.
3. ALB routes the request to the Amazon ECS Service.
4. Amazon ECS Service ensures the required ECS task is running.
5. The ECS Task running on AWS Fargate hosts the containerized web application.
6. The ECS Task pulls the latest application image (v2) from Amazon ECR.
7. The application processes the request and returns the response to the user.

---

## ☁️ AWS Services Used

- **Amazon ECS (Elastic Container Service)** – Container orchestration service used to run the application.
- **AWS Fargate** – Serverless compute engine for running containers without managing servers.
- **Amazon ECR (Elastic Container Registry)** – Stores Docker container images.
- **Application Load Balancer (ALB)** – Distributes incoming traffic to the ECS tasks.
- **Amazon VPC** – Provides networking for ECS resources.

---

## 📸 Project Screenshots

### Docker Image Build

![Docker Build](screenshots/docker-image-build.png)

### Docker Image Pushed to Amazon ECR

![ECR Repository](screenshots/ecr-image-push.png)

### ECS Service Deployment

![ECS Service](screenshots/ecs-service-deployment.png)

### Application Load Balancer

![Application Load Balancer](screenshots/application-load-balancer.png)

### Version 2 Application Deployment

![Application Version 2](screenshots/application-v2-deployment.png)

---

## 🎯 Project Outcome

- Successfully containerized a web application using Docker.
- Stored and managed container images in Amazon ECR.
- Deployed the application on Amazon ECS using AWS Fargate.
- Configured an Application Load Balancer to route user traffic.
- Demonstrated container image versioning by deploying application version v2.
- Validated successful application deployment through the ALB endpoint.
- Gained practical experience with container-based application deployment on AWS.

---

## 📚 Key Learnings

- Understanding Docker image creation and containerization concepts.
- Managing container images using Amazon ECR.
- Creating and configuring Amazon ECS clusters, task definitions, services, and tasks.
- Deploying serverless containers using AWS Fargate.
- Integrating ECS services with an Application Load Balancer.
- Updating applications using container image versioning.
- Understanding how ECS services maintain the desired number of running tasks.
- Learning the end-to-end workflow of deploying containerized applications on AWS.

---
