📦 CI CD Pipeline using GitHub Actions Docker Terraform and AWS EC2

🔷 Overview

This project demonstrates an end to end CI CD pipeline that automates building container images and deploying applications to a cloud server. It integrates continuous integration continuous deployment containerization and infrastructure validation into a unified workflow.

🔷 Objective

To design an automated pipeline that builds Docker images validates infrastructure and deploys applications to an AWS EC2 instance without manual intervention.

🔷 Tech Stack
Category	Tools Used
CI CD	GitHub Actions
Containerization	Docker
Registry	Docker Hub
Infrastructure	Terraform
Cloud	AWS EC2
Application	Python Flask

🔷 Pipeline Workflow
Code Push  
   ↓  
GitHub Actions Trigger  
   ↓  
Build Docker Image  
   ↓  
Push to Docker Hub  
   ↓  
Terraform Init and Plan  
   ↓  
SSH to EC2  
   ↓  
Stop and Remove Old Container  
   ↓  
Pull Latest Image  
   ↓  
Run New Container  
🔷 Application Details
Component	Description
Framework	Python Flask
Endpoint	Root endpoint returns response
Port	5000
Base Image	Python slim
🔷 Infrastructure Details
Component	Configuration
Instance Type	t3 micro
OS	Ubuntu
Ports Open	22 (SSH) 5000 (Application)
Access	Public IP
🔷 Key Features
Automated pipeline triggered on code push
Docker image build and registry push
Infrastructure validation using Terraform
Secure deployment using SSH and GitHub Secrets
Automatic container replacement on deployment
🔷 Key Challenges and Learnings
Resolved container port conflicts during redeployment
Managed container lifecycle effectively
Debugged CI pipeline failures and YAML issues
Implemented secure secret handling in GitHub
Understood integration between CI CD Docker and cloud
🔷 Outcome
Fully automated CI CD pipeline implemented
Zero manual deployment after initial setup
Application successfully deployed on AWS EC2
Real world DevOps workflow achieved
🔷 Limitations
Single instance deployment
No load balancing or scaling
No monitoring or logging integration
No rollback strategy
🔷 Future Improvements
Add load balancer and auto scaling
Integrate monitoring using CloudWatch
Implement blue green deployment
Use Terraform for full infrastructure automation
Move to Kubernetes for orchestration
🔷 Summary

This project establishes a strong foundation in CI CD by integrating GitHub Actions Docker Terraform and AWS EC2 into a single automated deployment pipeline. It reflects practical DevOps skills and can be extended into a production grade system.
