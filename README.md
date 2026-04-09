🚀 Spring Boot CI/CD Pipeline with Jenkins, SonarQube, Trivy & AKS
📌 Project Overview

This project demonstrates an end-to-end CI/CD pipeline for deploying a Java Spring Boot application to Azure Kubernetes Service (AKS) using modern DevOps tools and best practices.

The pipeline automates the complete workflow from code checkout → build → quality analysis → security scanning → containerization → deployment.

🛠️ Tech Stack
Version Control: Git, GitHub
Build Tool: Maven
CI/CD: Jenkins
Code Quality: SonarQube
Security Scanning: Trivy
Containerization: Docker
Container Registry: Azure Container Registry (ACR)
Orchestration: Azure Kubernetes Service (AKS)
CLI Tools: Azure CLI, kubectl 

🔄 CI/CD Pipeline Flow
GitHub → Jenkins → Maven Build → SonarQube Analysis → Docker Build → Trivy Scan → Push to ACR → Deploy to AKS

⚙️ Pipeline Stages
1. Checkout
Clones source code from GitHub repository.
2. Build
Compiles and packages the application using Maven.
3. Test
Executes unit tests (currently mocked/skipped for pipeline stability).
4. SonarQube Analysis
Performs static code analysis.
Detects bugs, vulnerabilities, and code smells.
Ensures code quality before proceeding further.
5. Docker Build
Builds Docker image of the Spring Boot application.
6. Trivy Scan
Scans Docker image for vulnerabilities.
Identifies security risks in OS packages and dependencies.
7. Push to ACR
Tags and pushes Docker image to Azure Container Registry.
8. Deploy to AKS
Deploys application using Kubernetes manifests.
Exposes application using LoadBalancer service.


🔐 Security & Best Practices
✅ Sensitive credentials (SonarQube token) stored securely in Jenkins
✅ No hardcoded secrets in pipeline
✅ Integrated security scanning using Trivy
✅ Modular and scalable pipeline design


🌐 Application Deployment
Application successfully deployed on AKS
Accessible via external LoadBalancer IP


📊 Key Features
Fully automated CI/CD pipeline
Integrated code quality checks (SonarQube)
Integrated container security scanning (Trivy)
Cloud-native deployment on Kubernetes
Production-like DevOps workflow

🚀 How to Run (High-Level)
Clone the repository
Configure Jenkins pipeline
Set up SonarQube and credentials
Build Docker image
Push image to ACR
Deploy to AKS using Kubernetes manifests

📈 Future Improvements
Implement Quality Gate enforcement in SonarQube
Fail pipeline on critical vulnerabilities in Trivy
Add Helm charts for deployment
Add monitoring (Prometheus + Grafana)


👩‍💻 Author
Jaismeen Kaur
DevOps & Cloud Enthusiast
