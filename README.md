🚀 Rancher on GitHub CodeSpaces
This repository provides a step-by-step guide to set up Rancher, a powerful Kubernetes management tool, on GitHub CodeSpaces. Rancher allows you to deploy, manage, and scale Kubernetes clusters efficiently, and running it inside GitHub CodeSpaces offers a cloud-based development environment for a seamless workflow.

📖 Table of Contents
Prerequisites
Setup Instructions
Usage
Troubleshooting
Connect with Me
✅ Prerequisites
To follow this guide, ensure you have:

A GitHub Account with CodeSpaces enabled.
Basic knowledge of Kubernetes and Docker.
An internet connection to pull the Rancher Docker image.
🚀 Setup Instructions
1. Create a GitHub Repository
Create a new repository on GitHub.
Clone this repository or start from scratch by initializing a README file.
2. Open CodeSpaces
Click on the Code button in GitHub and choose Open with CodeSpaces.
3. Install Docker in CodeSpaces
In the terminal of CodeSpaces, run the following commands to install Docker:

sudo apt-get update
sudo apt-get install -y docker.io
Verify Docker installation:

docker --version
4. Pull Rancher Docker Image
Run the following command to pull the latest Rancher image:

docker pull rancher/rancher:latest
5. Run Rancher
Start the Rancher container with the following command:

docker run -d --privileged --restart=unless-stopped -p 80:80 -p 443:443 rancher/rancher
6. Access Rancher UI
Once Rancher is running, open your browser and go to:

http://localhost
You should see the Rancher login page. Follow the steps to set up Rancher and start managing Kubernetes clusters.
