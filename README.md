📦CI CD Pipeline using GitHub Actions Docker Terraform and AWS EC2

---

## Overview
This project demonstrates an end to end CI CD pipeline that automates building container images and deploying applications to a cloud server. It integrates continuous integration continuous deployment containerization and infrastructure validation into a unified workflow.

---

## Objective
To design an automated pipeline that builds Docker images validates infrastructure and deploys applications to an AWS EC2 instance without manual intervention.

---

## Tech Stack

| Category          | Tools Used        |
|-------------------|------------------|
| CI CD             | GitHub Actions   |
| Containerization  | Docker           |
| Registry          | Docker Hub       |
| Infrastructure    | Terraform        |
| Cloud             | AWS EC2          |
| Application       | Python Flask     |

---

## Pipeline Workflow

---

## Application Details

| Component  | Description                        |
|------------|------------------------------------|
| Framework  | Python Flask                       |
| Endpoint   | Root endpoint returns response     |
| Port       | 5000                               |
| Base Image | Python slim                        |

---

## Infrastructure Details

| Component      | Configuration                  |
|----------------|-------------------------------|
| Instance Type  | t3 micro                      |
| OS             | Ubuntu                        |
| Ports Open     | 22 (SSH), 5000 (Application)  |
| Access         | Public IP                     |

---

## Key Features

- Automated pipeline triggered on code push  
- Docker image build and push to registry  
- Terraform based infrastructure validation  
- Secure deployment using SSH and GitHub Secrets  
- Automatic container replacement during deployment  

---

## Key Challenges and Learnings

- Resolved container port conflicts during redeployment  
- Managed container lifecycle effectively  
- Debugged CI pipeline and YAML issues  
- Implemented secure secret management  
- Integrated multiple DevOps tools into a single workflow  

---

## Outcome

- Fully automated CI CD pipeline  
- Zero manual deployment after setup  
- Application deployed successfully on AWS EC2  
- End to end DevOps workflow implemented  

---

## Limitations

- Single instance deployment  
- No load balancing or scaling  
- No monitoring or logging integration  
- No rollback strategy  

---

## Future Improvements

- Add load balancer and auto scaling  
- Integrate monitoring using CloudWatch  
- Implement blue green deployment  
- Use Terraform for full infrastructure provisioning  
- Move to Kubernetes for orchestration  

---

## Summary

This project demonstrates a complete CI CD workflow integrating GitHub Actions Docker Terraform and AWS EC2. It provides a strong foundation in automation deployment and real world DevOps practices.
