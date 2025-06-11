# 🍔 DevOps Project: Swiggy Clone CI/CD Pipeline

This project demonstrates an end-to-end DevOps CI/CD pipeline for a containerized Swiggy clone application. The pipeline integrates security, quality, and automation tools like SonarQube, Trivy, and OWASP, deployed and orchestrated using Jenkins and Terraform.

![image](https://github.com/user-attachments/assets/67ce3626-f6d1-407b-93a0-1c295bb2ebe0)

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

## CI/CD Pipeline in Jenkins
![image](https://github.com/user-attachments/assets/1249da3c-a6fe-4381-a809-3f81dc028d47)

## SonarQube Analysis
![image](https://github.com/user-attachments/assets/79c84b0c-d2b5-4eaa-af8e-a55105bb70d4)

---

## Trivy.txt

![image](https://github.com/user-attachments/assets/466f98e3-042e-4e40-81aa-f03fba9da743)

---

## Jenkins Plugin used
![image](https://github.com/user-attachments/assets/552b019a-324c-43fe-9068-57419ab57eee)
![image](https://github.com/user-attachments/assets/9648ad8a-46a1-42b4-ac67-4570e507f345)
![image](https://github.com/user-attachments/assets/43ae270c-26a1-42bf-b8f2-89500dd34fd9)
![image](https://github.com/user-attachments/assets/851cacb7-9578-47bb-a90c-816b0e259394)
![image](https://github.com/user-attachments/assets/da7b74cc-1c65-4068-8c1a-5407540c5cc2)
![image](https://github.com/user-attachments/assets/e2a58760-7ca5-446b-ba1b-c389e422256e)


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


