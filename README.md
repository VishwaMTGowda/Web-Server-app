# Static HTML Website with CI/CD

This is a simple static HTML website deployed automatically to AWS EC2 using GitHub Actions CI/CD pipeline.

## Features

- 🚀 **Automatic Deployment**: Deploys to EC2 on every push to main branch
- 🔒 **Branch Protection**: No direct pushes to main - PRs require approval
- ⚡ **Nginx Web Server**: Fast and reliable static file serving
- 📊 **Deployment Tracking**: Shows deployment time and commit info
- 🌐 **Live Updates**: Auto-deploys within seconds of merge

## Setup

1. **EC2 Instance**: Ubuntu with port 80 open
2. **GitHub Secrets**:
   - `EC2_SSH_KEY`: Private SSH key for EC2 access
   - `EC2_HOST`: EC2 public IP or domain

## Access

- Website: `http://EC2_IP`
- Deployment Info: `http://EC2_IP/deployment`
- JSON Info: `http://EC2_IP/info`

## CI/CD Pipeline

1. Push to feature branch
2. Create Pull Request
3. Get approval from collaborator
4. Merge to main
5. GitHub Actions deploys automatically
6. Website updates in seconds

   <img width="1887" height="942" alt="image" src="https://github.com/user-attachments/assets/52b06cd5-d985-41cc-8d59-c81dd6ab267c" />
