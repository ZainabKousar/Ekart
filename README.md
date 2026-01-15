🚀 Spring Boot Application – DevOps CI/CD & Kubernetes Deployment
📌 Project Overview

This repository demonstrates a complete DevOps deployment pipeline for a Spring Boot application.
The main focus of this project is automation, security, containerization, and Kubernetes deployment using real-world DevOps tools.

🏗️ Deployment Architecture

The application is deployed using a fully automated CI/CD pipeline:

Code is pushed to GitHub

Jenkins pipeline is triggered automatically

Application is built using Maven

Code quality is analyzed using SonarQube

Dependency vulnerabilities are scanned using OWASP

Docker image is built

Docker image is scanned using Trivy

Image is deployed to Kubernetes cluster

Application is exposed using Kubernetes Service

🧰 Tools Used for Deployment
🔹 CI/CD & Build

GitHub – Source code repository

Jenkins – CI/CD automation

Maven – Build and packaging

🔹 Security & Quality

SonarQube – Static code analysis

OWASP Dependency Check – Dependency vulnerability scan

Trivy – Container image vulnerability scanning

🔹 Container & Orchestration

Docker – Application containerization

Kubernetes (kubeadm cluster) – Container orchestration

Calico – Networking

ServiceAccount & RBAC – Secure cluster access

🔹 Infrastructure

AWS EC2 – Jenkins server and Kubernetes nodes

Security Groups – Network access control

⚙️ Jenkins CI/CD Pipeline Details

The Jenkins pipeline performs the following stages:

Source Code Checkout

Pulls code from GitHub repository

Build Stage

Builds the application using Maven

Code Quality Analysis

Runs SonarQube analysis to detect bugs and code smells

Security Scan (Dependencies)

Runs OWASP Dependency Check to find known vulnerabilities

Docker Image Build

Builds Docker image using Dockerfile

Container Image Scan

Scans Docker image using Trivy for CVEs

Push Image

Pushes Docker image to Docker Hub

Kubernetes Deployment

Applies Kubernetes YAML files using kubectl

Deploys application pods and services

🔐 Kubernetes Access & Security

Jenkins runs on a separate server

Kubernetes cluster is accessed securely using:

ServiceAccount

ClusterRole & ClusterRoleBinding

Jenkins does not use admin credentials

Access is restricted using RBAC best practices

☸️ Kubernetes Resources Used

Namespace – Logical isolation

Deployment – Manages pods and replicas

Service (NodePort / LoadBalancer) – Exposes application

ServiceAccount – Jenkins authentication

RBAC – Permission control

🌐 Application Exposure

Application is exposed using:

NodePort (30000–32767) or

LoadBalancer (cloud-based)

Security groups allow required ports only

Accessed via:

http://<Node_Public_IP>:<NodePort>

🧪 Verification & Monitoring

kubectl get nodes – Cluster health

kubectl get pods – Pod status

kubectl get svc – Service exposure

Jenkins build logs for pipeline validation

🎯 Key DevOps Highlights

End-to-end automated CI/CD pipeline

Secure Kubernetes access using RBAC

Integrated security scanning at multiple stages

Production-like Kubernetes deployment

Separate Jenkins and Kubernetes servers

📌 Use Case

This project demonstrates real-world DevOps deployment skills including:

CI/CD automation

Kubernetes deployments

Container security

Cloud infrastructure usage

<img width="1920" height="1080" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/144463c4-626a-4f3c-b3fc-83025275e469" />


<img width="1920" height="1080" alt="Screenshot (33)" src="https://github.com/user-attachments/assets/a355eca3-2ad3-47aa-9b0b-2e430618b945" />

<img width="1920" height="1080" alt="Screenshot (35)" src="https://github.com/user-attachments/assets/6f74ced5-2486-45a8-b10e-d9e4881c4b12" />

<img width="1920" height="1080" alt="Screenshot (36)" src="https://github.com/user-attachments/assets/4e5eebae-3f02-451c-ba29-9e2d1795229c" />

<img width="1920" height="1080" alt="Screenshot (37)" src="https://github.com/user-attachments/assets/18475c0a-befd-4d3d-ac45-83dae22e3b36" />

<img width="1920" height="1080" alt="Screenshot (10)" src="https://github.com/user-attachments/assets/3a19ed2c-dc04-45eb-88c2-5d582503fb40" />

<img width="1920" height="1080" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/43438bc8-b5ee-46b8-9ae5-ef4af700888d" />

<img width="1920" height="1080" alt="Screenshot (15)" src="https://github.com/user-attachments/assets/49c00c85-d53a-4c2e-99b6-9e810bf6e57e" />

<img width="1920" height="1080" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/16e0d183-3cfc-491c-b92f-3674c96c88f1" />

<img width="1920" height="1080" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/79ad550d-636b-490f-b455-631d7ea9235d" />
