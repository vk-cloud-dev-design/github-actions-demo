# GitHub Actions & Azure DevOps CI/CD Demo

This repository is created for learning and practicing CI/CD using GitHub Actions and Azure DevOps.

## 🎯 Objective

The objective of this project is to understand the complete CI/CD lifecycle:

```text
Developer
    ↓
GitHub Repository
    ↓
CI Pipeline
    ↓
Build
    ↓
Test
    ↓
Artifact
    ↓
Deployment
    ↓
Azure
```

## 🛠️ Technologies

* Git
* GitHub
* GitHub Actions
* YAML
* Azure
* Azure DevOps
* Azure DevOps Classic Pipeline
* Azure DevOps YAML Pipeline

## 📁 Project Structure

```text
github-actions-demo/
│
├── app/
│   └── index.html
│
├── tests/
│   └── test.sh
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
└── README.md
```

## 🔄 CI/CD Learning Path

### Phase 1 — Git & GitHub

* Create repository
* Create branches
* Commit changes
* Push changes
* Create Pull Requests
* Merge changes

### Phase 2 — GitHub Actions

* Workflow
* Events and triggers
* Jobs
* Steps
* Actions
* Runners
* Build
* Test
* Artifacts
* Variables
* Secrets
* Environments
* Manual execution
* Pull Request workflows
* Scheduled workflows
* Job dependencies
* Conditions
* Matrix builds

### Phase 3 — Azure Deployment

```text
GitHub
   ↓
GitHub Actions
   ↓
Build
   ↓
Test
   ↓
Artifact
   ↓
Azure
   ↓
Application Deployment
```

### Phase 4 — Azure DevOps Classic Pipeline

```text
GitHub
   ↓
Azure DevOps
   ↓
Classic Build Pipeline
   ↓
Build
   ↓
Test
   ↓
Publish Artifact
   ↓
Classic Release Pipeline
   ↓
Dev
   ↓
QA
   ↓
Production
```

### Phase 5 — Azure DevOps YAML Pipeline

The final goal is to recreate the Classic Pipeline using an Azure DevOps YAML pipeline.

## 📚 Key CI/CD Concepts

| Concept            | Description                                   |
| ------------------ | --------------------------------------------- |
| Repository         | Stores source code                            |
| Workflow           | GitHub Actions automation                     |
| Job                | Collection of related steps                   |
| Step               | Individual pipeline operation                 |
| Action             | Reusable automation component                 |
| Runner             | Machine that executes the workflow            |
| Artifact           | Build output used for deployment              |
| Environment        | Deployment target                             |
| Secret             | Securely stored sensitive value               |
| Service Connection | Authentication between Azure DevOps and Azure |

## 🚀 Final Architecture

```text
                    Developer
                        │
                        │ git push
                        ▼
                ┌───────────────┐
                │    GitHub     │
                │  Repository   │
                └───────┬───────┘
                        │
                        ▼
              ┌───────────────────┐
              │  GitHub Actions   │
              │                   │
              │  Checkout         │
              │  Build            │
              │  Test             │
              │  Package          │
              │  Artifact         │
              └─────────┬─────────┘
                        │
                        ▼
                    Artifact
                        │
                        ▼
                  Azure Deployment
                        │
                 ┌──────┴──────┐
                 ▼             ▼
                Dev           QA
                               │
                               ▼
                          Production
```

## 📌 Status

This repository is being developed as a hands-on DevOps learning project.

The pipeline will be built incrementally, starting with GitHub Actions and then moving to Azure DevOps Classic and YAML pipelines.

