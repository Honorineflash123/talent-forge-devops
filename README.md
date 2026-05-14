# talent-forge-devops Documentation

Talent Forge DevOps Pipeline Technical
Documentation
Author: Asobo Honorine Wehpon


PROJECT : DevOps My App — Dockerized Web App with CI/CD Pipeline

Project Overview: This project demonstrates a real-world DevOps workflow using:

- Git & GitHub
- Docker
- Docker Hub
- GitHub Actions (CI/CD)
- Render Cloud Hosting
- UptimeRobot Monitoring.

       This application is a lightweight static status page hosted inside an Nginx Docker container and automatically deployed through a CI/CD pipeline. The following tools and the exact purpose why the were used is as follows:

| Tool                                     |  Purpose |

| GitHub                               | Version control & repository hosting |
| GitHub Actions                  | CI/CD automation |
| Docker                                | Containerization |
| Docker Hub                       | Container image registry |
| Render                                | Cloud hosting |
| UptimeRobot                     | Monitoring & uptime alerts |
| Nginx                                  | Web server |




Live Project Links

 GitHub Repository :  https://github.com/Honorineflash123/talent-forge-dev

DockerhubRepository: 

https://hub.docker.com/repository/docker/hnorinewehpon/myapp/general



Live Render URL:  https://myapp-latest-f1gt.onrender.com


             Project Structure

talent-forge-devops/
│
├── .github/
│   └── workflows/
│       └── deploy.yml
│
├── Dockerfile
├── index.html
└── README.md

GitHub Secrets Used
The following secrets were configured securely in Github: 
DOCKER_USERNAME
DOCKER_PASSWORD
DevOps Workflow Architecture

                ┌────────────────────┐
                │   Developer Code   │
                │  (index.html edit) │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │     GitHub Repo    │
                │   Push to main     │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ GitHub Actions CI  │
                │ Build Docker Image │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │    Docker Hub      │
                │ Store Docker Image │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │      Render        │
                │ Deploy Container   │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │   Live Web App     │
                │   Public Internet  │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │   UptimeRobot      │
                │ Monitoring & Alert │
                └────────────────────┘


CI/CD Pipeline Flow
Code Change
    │
  Git Push to Main
    │
    ▼
GitHub Actions Triggered
    │
    ▼
Docker Image Built
    │
    ▼
Docker Image Pushed to Docker Hub
    │
    ▼
Render Pulls Latest Image
    │
    ▼
Application Redeployed
    │
    ▼
UptimeRobot Monitors Availability

What I Learned from this project  and future improvements

Through this project, I gained hands-on experience with:
    • DevOps fundamentals 
    • GitHub workflow automation 
    • Docker containerization 
    • CI/CD pipeline implementation 
    • Cloud deployment 
    • Monitoring & uptime management 
      And some of the Future Improvements I will be practicing include:
    • Add multi-page website 
    • Add health check endpoint 
    • Add automated testing workflow 
    • Implement Kubernetes deployment 
    • Add custom domain 

