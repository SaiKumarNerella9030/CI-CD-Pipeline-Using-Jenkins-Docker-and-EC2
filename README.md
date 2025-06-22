# CI/CD Pipeline Using Jenkins, Docker, and EC2

This project demonstrates a complete CI/CD pipeline for a containerized Node.js application using **Jenkins**, **Docker**, and **AWS EC2**. The pipeline automates cloning from GitHub, Docker image build, and deployment to a live EC2 instance.

---

## 🚀 Technologies Used

- **Jenkins** – Orchestrates the CI/CD pipeline
- **Docker** – Builds and runs the application container
- **GitHub** – Hosts the source code and `Jenkinsfile`
- **AWS EC2** – Hosts Jenkins and runs the deployed container

---

## 📁 Project Structure

├── app.js # Node.js app (Express server)
├── Dockerfile # Docker image instructions
├── Jenkinsfile # Jenkins CI/CD pipeline definition
├── package.json # App metadata and dependencies

After deployment, visit:
http://<EC2-PUBLIC-IP>:3000
