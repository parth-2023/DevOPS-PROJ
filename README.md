# 🎟️ BMS-CLONE: A Ticketing App with DevOps Integration

[![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen)]()
[![Deployment Status](https://img.shields.io/badge/Deployment-Success-blue)]()
[![Monitored with](https://img.shields.io/badge/Monitored_with-Prometheus%20%26%20Grafana-orange)]()

## 📌 Table of Contents

- [About the Project](#about-the-project)
  - [Built With](#built-with)
  - [Project Scope](#project-scope)
- [DevOps Pipeline](#devops-pipeline)
  - [CI/CD Pipeline](#cicd-pipeline)
  - [Infrastructure Overview](#infrastructure-overview)
  - [Monitoring Stack](#monitoring-stack)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## 🚀 About the Project

**BMS-CLONE** is a responsive frontend ticket booking platform inspired by modern platforms like BookMyShow. The aim of the project is to demonstrate a full DevOps lifecycle implementation using tools like Jenkins, Docker, Kubernetes, and AWS.

This project focuses on deploying the frontend using an automated CI/CD pipeline integrated with security checks and monitoring tools.

### 🛠 Built With

- **Frontend**: HTML, CSS, JavaScript  
- **Containerization**: Docker  
- **CI/CD**: Jenkins  
- **Security Scans**: SonarQube, Trivy, OWASP ZAP  
- **Orchestration**: Kubernetes  
- **Cloud**: AWS (EC2, Route 53, Load Balancer)  
- **Monitoring**: Prometheus + Grafana  

### 🔍 Project Scope

This project includes only the **frontend** of the BMS-CLONE platform and focuses on its automated deployment using modern DevOps practices. Backend functionality is outside the current scope.

---

## ⚙️ DevOps Pipeline

The DevOps workflow is designed to reflect real-world CI/CD pipelines for production applications.

### 🔗 CI/CD Pipeline

- **Source Code**: Pulled from GitHub
- **Code Quality Analysis**: Performed via SonarQube
- **Security Scanning**:
  - **OWASP ZAP** for app-level vulnerabilities
  - **Trivy** for Docker image scanning
- **Dockerization**: Application packaged into a Docker container
- **Testing**: Smoke tests run inside container
- **Deployment**: Container deployed to Kubernetes cluster
- **Notifications**: Email alerts on pipeline status

### 🏗 Infrastructure Overview

Deployed on AWS with the following setup:

- **EC2 Instances** hosting Jenkins, SonarQube, and Kubernetes cluster
- **Kubernetes Cluster** manages containers for the BMS-CLONE frontend
- **Docker Hub** used as image registry
- **AWS Load Balancer** distributes traffic
- **Custom Domain via Route 53** for external access

### 📊 Monitoring Stack

- **Prometheus**: Collects cluster and app metrics
- **Grafana**: Dashboards to monitor performance and alerts

---

## 💡 Usage

After deployment, users can:

- View upcoming events across categories like music, theatre, and sports
- See event details such as time, location, and description

*Note: Checkout, payment, and backend features are not included in this version.*

---

## 🗺 Roadmap

- Add backend microservices for seat selection, payment, and booking
- User authentication and profile management
- Role-based access for event organizers
- Deploy complete microservice architecture

---

## 🤝 Contributing

Contributions are welcome! Here's how to get started:

1. Fork this repository
2. Create a new branch (`git checkout -b feature/new-feature`)
3. Make your changes
4. Commit and push (`git commit -m 'Add feature'` → `git push origin`)
5. Submit a pull request

---

## 📄 License

Distributed under the MIT License. See `LICENSE.txt` for more info.

---

## 📬 Contact

**Parth Gupta**  
Email: [parth.gupta2023c@vitstudent.ac.in]

---

## Acknowledgments 🙏
* This is part of a **1-month IBM DevOps Certification**.
