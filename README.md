# DevSecOps Pipeline 🔐🚀

## Overview
Complete DevSecOps pipeline with automated security 
scanning at every stage of CI/CD.

## Security Stages
| Stage | Tool | Purpose |
|---|---|---|
| SAST | Bandit | Python code security scan |
| Dependency Check | Safety | Vulnerable packages detect |
| Image Scan | Trivy | Docker vulnerabilities scan |
| Deploy | GitHub Actions | Auto deploy to EC2 |

## Pipeline Flow

Code Push

↓

SAST Scan (Bandit)

↓

Dependency Check (Safety)

↓

Docker Image Scan (Trivy)

↓

Build + Push to DockerHub

↓

Deploy to EC2

## Tech Stack
Bandit | Safety | Trivy | Docker | 
GitHub Actions | AWS EC2 | Python Flask
