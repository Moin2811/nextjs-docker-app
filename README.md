
## 🚀 Next.js Application Deployment with Docker, GitHub Actions, and Kubernetes (Minikube on AWS EC2)


## 📘 Project Overview

This project demonstrates the complete DevOps workflow of containerizing, automating, and deploying a modern web application.

I created a Next.js application, containerized it using Docker, automated the build and push process with GitHub Actions, and deployed it to a Kubernetes cluster (Minikube) running on an AWS EC2 instance.

The main goal of this project was to gain hands-on experience in building containerized applications, setting up CI/CD pipelines, and deploying applications in Kubernetes.

## 🎯 Objectives

Containerize a Next.js application using Docker

Automate the build and push process using GitHub Actions and GitHub Container Registry (GHCR)

Deploy the containerized application on Kubernetes (Minikube)

Access the deployed application through a web browser

## 🧩 Project Architecture

The workflow begins with a Next.js web application that is containerized using Docker.
A GitHub Actions workflow is used to automatically build and push the Docker image to the GitHub Container Registry.
Once the image is available, it is deployed to a Kubernetes cluster using deployment and service manifests.
Finally, the application is exposed via NodePort or port forwarding for browser access.

## ⚙️ Tools & Technologies Used

Next.js

Docker

GitHub Actions

GitHub Container Registry (GHCR)

Kubernetes (Minikube)

AWS EC2 (Ubuntu Server)

YAML Manifests for deployment and service configuration

## 🧱 Setup Summary

Cloned the repository and created a simple Next.js application using the official starter template.

Wrote a Dockerfile to containerize the application, ensuring efficient layer caching and production best practices.

Created a GitHub Actions workflow to automatically build and push the Docker image to GitHub Container Registry on every push to the main branch.

Deployed the application on Minikube using Kubernetes manifests — one for Deployment (defining pods and replicas) and one for Service (to expose the app).

Accessed the application by forwarding the Minikube port or exposing it through NodePort on AWS EC2.

## ☸️ Kubernetes Deployment Summary

The Kubernetes setup consisted of two YAML manifests:

Deployment Manifest: Defined the number of replicas, container image, and health checks for the Next.js application.

Service Manifest: Exposed the application on a specific port using the NodePort service type, allowing external access.

After applying these manifests, the application was successfully deployed to the Minikube cluster.

## 🌍 Accessing the Application

The deployed Next.js application was accessed through port forwarding and NodePort.

On the AWS EC2 instance, port 3000 was opened in the Security Group settings to allow external access.
Once port forwarding was established, the application became accessible via the EC2 public IP address in a web browser.

## ✅ Results

The Next.js application was successfully containerized and deployed.

The CI/CD pipeline using GitHub Actions and GHCR automated the image build and push process.

The Kubernetes deployment on Minikube worked seamlessly on the AWS EC2 environment.

The application was successfully accessible from a browser through port forwarding or NodePort exposure.

## 🧠 Learning Outcomes

Through this project, I gained practical experience in:

Building Docker images and optimizing container builds

Automating continuous integration and deployment using GitHub Actions

Managing Kubernetes workloads and services

Configuring Minikube and handling image pull authentication issues

Exposing applications securely on AWS EC2 environments

## Screenshots
## Webpage Running

<img width="1918" height="1020" alt="Screenshot 2025-10-06 163153" src="https://github.com/user-attachments/assets/f2bc8ad8-4683-49f6-9fd7-a125fb67c959" />
<img width="1918" height="1008" alt="Screenshot 2025-10-06 214826" src="https://github.com/user-attachments/assets/c8ed8502-333e-448a-8cdf-20fc3138ce4c" />
<img width="1918" height="1012" alt="Screenshot 2025-10-06 214904" src="https://github.com/user-attachments/assets/7d8bb98d-4916-47fb-b8a2-b9561f1fe49b" />


🌐 Repository & Image Links

Repository URL: https://github.com/Moin2811/nextjs-docker-app.git

GHCR Image URL:ghcr.io/moin2811/nextjs-docker-app:latest


## 📜 Author

Mohammed Moin Raoof

DevOps Enginner


