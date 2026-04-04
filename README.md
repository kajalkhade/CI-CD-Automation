🚀 End-to-End CI/CD Pipeline using Jenkins, Docker, and AWS EC2
📌 Project Overview

This project demonstrates the implementation of a complete CI/CD (Continuous Integration and Continuous Deployment) pipeline to automate the deployment of a Node.js application using Jenkins, Docker, and AWS EC2.

The pipeline ensures faster, consistent, and reliable application delivery by automating build, test, and deployment processes.


🛠️ Tech Stack
CI/CD Tool: Jenkins
Containerization: Docker
Cloud Platform: AWS EC2 (Ubuntu)
Version Control: GitHub
Backend: Node.js


⚙️ Features
Automated build and deployment process
Integration with GitHub for continuous integration
Docker-based containerized deployment
Secure AWS EC2 setup with configured security groups
Reduced manual effort and faster release cycles


🏗️ Architecture
Developer pushes code to GitHub
Jenkins detects changes using webhook
Jenkins builds the project
Docker image is created
Container is deployed on AWS EC2


🚀 Setup & Installation
1️⃣ Launch EC2 Instance
Create Ubuntu EC2 instance
Configure security groups (allow ports: 22, 8080, 80)


2️⃣ Install Jenkins
sudo apt update
sudo apt install openjdk-11-jdk -y
sudo apt install jenkins -y


3️⃣ Install Docker
sudo apt install docker.io -y
sudo usermod -aG docker jenkins
sudo systemctl restart jenkins


4️⃣ Configure Jenkins
Access Jenkins via: http://<EC2-IP>:8080
Install required plugins
Connect with GitHub repository


5️⃣ Create Jenkins Pipeline
Add Jenkinsfile in repo
Configure pipeline job


📦 Deployment
On every code push, Jenkins automatically:
Pulls latest code
Builds Docker image
Runs container on EC2


📈 Outcome
Fully automated deployment pipeline
Reduced deployment time
Improved reliability and consistency


