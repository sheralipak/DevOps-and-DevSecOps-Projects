# Project 1: End-to-End DevSecOps & GitOps Pipeline on Kubernetes

A production-grade microservices deployment pipeline featuring automated CI/CD security scanning, GitOps continuous delivery, and real-time cluster observability.

---

##  Architecture Overview

```text
[ Developer Commit ] ──► [ Jenkins CI ] ──► [ SonarQube Scan ] ──► [ Trivy Scan ]
                                                                       │
[ Grafana Dashboard ] ◄── [ Prometheus ] ◄── [ ArgoCD GitOps ] ◄── [ Docker Hub ]
🛠️ Tech Stack & Services
CI Automation: Jenkins

Code Security: SonarQube (Static Analysis)

Container Security: Trivy Vulnerability Scanner

Container Registry: Docker Hub

Continuous Delivery: ArgoCD (GitOps Operator)

Orchestration: Kubernetes (Minikube)

Observability: Prometheus & Grafana

💡 Key Highlights
Shift-Left Security: Automated security gates in Jenkins prevent vulnerable code and images from entering production.

Declarative GitOps: Managed state synchronization zero-drift using ArgoCD.

Full Observability: Live metrics scraping in Prometheus with HTTP traffic visualization on Grafana dashboards.
