
## 🚀 CI/CD Status
![Build & Deploy](https://github.com/ritesh355/portfolio/tree/main/.github/workflows/main.yml/badge.svg)

## 🔄 Deployment Workflow
```mermaid
flowchart LR
    A[Push to GitHub] --> B[GitHub Actions]
    B --> C[Build & Test]
    C --> D[Docker Build]
    D --> E[Push to Docker Hub]
    E --> F[EC2 Pull Latest Image]
    F --> G[Restart Container]
    G --> H[Portfolio Live 🚀]
