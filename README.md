🚀 AWS DevOps CI/CD Pipeline
This project demonstrates a complete CI/CD pipeline built with AWS DevOps tools and Terraform. It automates the end-to-end software delivery process — from source code integration to build, artifact storage, and deployment to EC2 — using AWS-native services and Infrastructure as Code.

🔧 Tech Stack
Source Control: GitHub (via AWS CodeStar Connection)

CI/CD: AWS CodePipeline + CodeBuild + CodeDeploy

IaC: Terraform

Artifact Store: Amazon S3

Deployment Target: EC2 Instances

📂 Project Structure
bash
Copy
Edit
aws-devops-pipeline/
├── terraform/       # Infrastructure as Code (CodePipeline, IAM, EC2)
├── app/             # Sample application with buildspec.yml
├── scripts/         # Deployment or setup scripts
⚙ Pipeline Flow
Code is pushed to GitHub → triggers CodePipeline

CodeBuild builds app + stores artifacts in S3

CodeDeploy deploys app to EC2

Optional: add static code analysis, tests, and security scans

✅ Features
Infrastructure managed by Terraform

Versioned artifact storage in S3

Deployment to EC2 with CodeDeploy

Easily customizable for containerized workflowsREADME File
