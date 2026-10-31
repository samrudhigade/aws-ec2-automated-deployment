AWS EC2 Automated Deployment Using Jenkins

Project Overview
This project demonstrates an automated Continuous Integration and Continuous Deployment (CI/CD) pipeline using Jenkins and AWS EC2.

The pipeline automatically fetches website source code from GitHub, validates the required files, packages the website, and deploys it to an Apache web server hosted on an AWS EC2 instance.

Project Objective
To automate the website deployment process using Jenkins and AWS EC2, reducing manual effort and improving deployment efficiency.

Technologies Used
- Cloud Platform: Amazon Web Services (AWS)
- Compute Service: Amazon EC2
- CI/CD Tool: Jenkins
- Version Control: Git and GitHub
- Operating System: Ubuntu Linux
- Web Server: Apache
- Scripting: Shell Scripting
- Secure Communication: SSH

Architecture

GitHub → Jenkins Server (EC2) → Build & Package → SSH Deployment → Web Server (EC2) → Website

 CI/CD Pipeline Stages

1. Checkout: Jenkins retrieves the source code from the GitHub repository.
2. Validate: Checks whether the required website files are available.
3. Package: Creates a compressed archive of the website files.
4. Deploy: Transfers the website package to the Web Server EC2 instance using SSH.
5. Verify: Checks whether the deployed website is accessible.

Project Structure

```text
aws-ec2-automated-deployment/
│
├── Jenkinsfile
├── README.md
│
└── website/
    ├── index.html
    └── style.css
```

How It Works

- Source code is maintained in GitHub.
- Jenkins connects to the GitHub repository.
- The pipeline executes the defined stages automatically when triggered.
- Website files are packaged and transferred to the Web Server EC2 instance.
- Apache serves the deployed website.

Learning Outcomes

- Hands-on experience with Jenkins pipeline creation.
- GitHub integration with Jenkins.
- AWS EC2 instance management.
- Automated website deployment.
- SSH-based remote server communication.
- Basic CI/CD workflow implementation.


