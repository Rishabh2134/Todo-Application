📝 Todo Application – CI/CD on GKE

A lightweight Flask-based Todo Application with an end-to-end CI/CD pipeline using Jenkins, Docker, and Google Kubernetes Engine (GKE). The pipeline supports automated Docker image builds and deployments to a GKE cluster with one click.

🚀 Features
🧾 Create, complete, and delete todo tasks

🐳 Dockerized Flask app

🔁 CI/CD via Jenkins declarative pipeline

☸️ One-click deployment to GKE

🔐 Secrets management with Jenkins credentials

🔄 sed-based tag substitution for versioning

📁 Folder Structure
.
├── app.py                 # Main Flask application
├── templates/             # HTML templates
├── instance/              # Flask config
├── Dockerfile             # Image build config
├── Jenkinsfile            # CI/CD pipeline config
├── Deployment.yaml        # K8s manifest (template)
└── .circleci/config.yml   # Optional: CircleCI support

🛠 Tech Stack
Layer	        Technology
Application	    Flask (Python)
CI/CD	        Jenkins + Declarative Pipeline
Container	    Docker
Orchestration	Kubernetes (GKE)
Registry	    DockerHub

✅ CI/CD Workflow
Clone the repository from GitHub

Build the Docker image locally

Push the image to DockerHub

Replace tagversion with latest in your Kubernetes YAML

Deploy the updated YAML to Google Kubernetes Engine

⚙️ Prerequisites
GCP project and GKE cluster created

DockerHub account

Jenkins configured with:

Docker installed

Kubernetes CLI Plugin and Google Kubernetes Engine Plugin

Credentials stored securely for:

DockerHub (Docker_Password)

GKE access (Credentials)

Permissions and RBAC set correctly in GKE