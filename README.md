# AWS Static Website Deployment Pipeline

This project is my first end-to-end DevOps project. I built a personal portfolio website and deployed it on AWS using a CI/CD pipeline with GitHub Actions.

The main goal of this project was to understand how code can automatically move from GitHub to a live website without manual deployment.

---
## Portfolio Website

![Portfolio Homepage](screenshots/homepage.png)

## What this project does

Whenever I push changes to the `main` branch:

- GitHub Actions starts automatically.
- The website files are uploaded to an Amazon S3 bucket.
- CloudFront cache is cleared.
- The latest version of the website becomes live.

This means I only need to push my code to GitHub, and the deployment happens automatically.

---

## Technologies Used

- HTML
- CSS
- JavaScript
- Git
- GitHub
- GitHub Actions
- AWS S3
- Amazon CloudFront
- AWS IAM

---

## Project Workflow

```
Code Changes
      ↓
Git Push
      ↓
GitHub Repository
      ↓
GitHub Actions
      ↓
Amazon S3
      ↓
CloudFront
      ↓
Live Website
```

---

## Project Structure

```
portfolio-website/
│
├── index.html
├── css/
├── js/
├── assets/
├── .github/
│   └── workflows/
├── README.md
└── LICENSE
```

---

## GitHub Secrets Used

For security, I stored the AWS credentials as GitHub Secrets instead of writing them directly in the workflow.

- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- AWS_REGION
- S3_BUCKET
- CLOUDFRONT_DISTRIBUTION_ID

---

## What I Learned

While building this project, I learned:

- Hosting a static website on Amazon S3
- Using CloudFront to serve content
- Creating a simple CI/CD pipeline with GitHub Actions
- Managing AWS permissions using IAM
- Storing sensitive credentials securely with GitHub Secrets
- Automating deployments instead of uploading files manually

---

## Future Improvements

Some things I want to add in the future:

- Infrastructure provisioning with Terraform
- Configuration management using Ansible
- Containerization with Docker
- Deploying on Kubernetes (Amazon EKS)
- Monitoring and logging

---

## Live Demo

🌐 https://papersless.xyz

---

## Screenshots

I'll add screenshots of:

- Portfolio Website
- GitHub Actions Workflow
- Amazon S3 Bucket
- CloudFront Distribution

---

## Connect with Me

**Gagan Biswas**

- GitHub: https://github.com/sky7-devops
- LinkedIn: https://www.linkedin.com/in/gagan-biswas/
- Portfolio: https://papersless.xyz