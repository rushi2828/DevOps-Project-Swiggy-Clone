# 🍔 DevOps Project: Swiggy Clone CI/CD Pipeline

This project demonstrates an end-to-end DevOps CI/CD pipeline for a containerized Swiggy clone application. The pipeline integrates security, quality, and automation tools like SonarQube, Trivy, and OWASP, deployed and orchestrated using Jenkins and Terraform.

![image](https://github.com/user-attachments/assets/67ce3626-f6d1-407b-93a0-1c295bb2ebe0)

---

## CI/CD Pipeline in Jenkins
![image](https://github.com/user-attachments/assets/1249da3c-a6fe-4381-a809-3f81dc028d47)

## SonarQube Analysis
![image](https://github.com/user-attachments/assets/79c84b0c-d2b5-4eaa-af8e-a55105bb70d4)

---

## 🚀 Tech Stack & Tools Used

| Tool       | Purpose                            |
|------------|------------------------------------|
| **Terraform** | Infrastructure provisioning         |
| **GitHub**   | Source code management (SCM)       |
| **Jenkins**  | CI/CD orchestration                |
| **SonarQube**| Code quality and static analysis   |
| **OWASP ZAP**| Dynamic application security testing (DAST) |
| **Trivy**    | Container vulnerability scanning   |
| **Docker**   | Containerization                   |
| **DockerHub**| Container image registry           |

---

## 🛠️ Pipeline Stages Overview

1. **Code Checkout** from GitHub
2. **Build Docker Image** using Dockerfile
3. **Run Static Code Analysis** using SonarQube
4. **Run Security Scans** using:
   - **Trivy** for image scanning
   - **OWASP ZAP** for dynamic vulnerability testing
5. **Push Docker Image** to DockerHub
6. **Deploy to Test/Prod** using Jenkins & Docker

---

## ⚙️ Infrastructure Setup (via Terraform) : [terraform-ec2-sg](https://github.com/rushi2828/terraform-ec2-sg.git)

```bash
cd terraform/
terraform init
terraform plan
terraform apply
```
---


