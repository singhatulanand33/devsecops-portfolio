<div align="center">

# 🛡️ Atul Anand Singh
### **DevSecOps Engineer | Cloud Security Specialist | CI/CD & GitOps Architect**

<p align="center">
  <a href="https://github.com/singhatulanand33"><img src="https://img.shields.io/badge/GitHub-singhatulanand33-181717?style=for-the-badge&logo=github" alt="GitHub" /></a>
  <a href="https://linkedin.com/in/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin" alt="LinkedIn" /></a>
  <a href="mailto:singh.atulanand33@gmail.com"><img src="https://img.shields.io/badge/Email-singh.atulanand33%40gmail.com-EA4335?style=for-the-badge&logo=gmail" alt="Email" /></a>
  <a href="https://singhatulanand33.github.io/devsecops-portfolio"><img src="https://img.shields.io/badge/Live%20Portfolio-Visit%20Website-10B981?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
</p>

<p align="center">
  <b>"Shifting Security Left • Automating Continuous Compliance • Hardening Cloud Infrastructure"</b>
</p>

---

</div>

## 📌 Executive Summary

Passionate **DevSecOps & Cloud Security Engineer** dedicated to bridging the gap between Software Development, Security, and IT Operations. Specialized in architecting enterprise-grade, automated CI/CD pipelines that integrate robust security gates (SAST, DAST, SCA, Container Vulnerability Assessment, and IaC Compliance) without slowing down developer velocity.

- 🔒 **Core Focus:** Shift-Left Security, Zero-Trust Architecture, Kubernetes Runtime Defense, Automated Compliance.
- ☁️ **Cloud & Infra:** AWS, Kubernetes (EKS/K8s), Docker, Terraform, Helm, Linux Hardening.
- 🚀 **Automation & CI/CD:** GitHub Actions, Jenkins, GitLab CI, ArgoCD (GitOps).
- 🛡️ **Security Tooling:** SonarQube, Trivy, Snyk, OWASP ZAP, Checkov, Gitleaks, HashiCorp Vault, Falco.

---

## 🔄 End-to-End DevSecOps Pipeline Architecture

Below is the automated Shift-Left security pipeline model implemented across my projects:

```mermaid
flowchart LR
    A["💻 Developer Commit"] --> B["🔍 Pre-Commit\n(Gitleaks / Pre-commit)"]
    B --> C["⚙️ CI Pipeline\n(GitHub Actions / Jenkins)"]
    C --> D["📊 SAST & Code Quality\n(SonarQube / Semgrep)"]
    D --> E["📦 SCA & Dependencies\n(Trivy / OWASP Dep-Check)"]
    E --> F["🐳 Container Build\n& Image Scan (Trivy)"]
    F --> G["📜 IaC Security & Policy\n(Checkov / tfsec / OPA)"]
    G --> H["☸️ GitOps Deployment\n(ArgoCD to K8s / AWS)"]
    H --> I["⚡ DAST Scanning\n(OWASP ZAP)"]
    I --> J["🛡️ Runtime Security & Audit\n(Falco, Prometheus, Grafana)"]

    classDef dev fill:#1e293b,stroke:#3b82f6,stroke-width:2px,color:#fff;
    classDef sec fill:#0f172a,stroke:#ef4444,stroke-width:2px,color:#fff;
    classDef ops fill:#1e293b,stroke:#10b981,stroke-width:2px,color:#fff;

    class A,C dev;
    class B,D,E,G,I,J sec;
    class F,H ops;
```

---

## 🛠️ Technical Competency Matrix

| Domain | Tools & Technologies |
| :--- | :--- |
| **Cloud Providers** | AWS (IAM, EKS, VPC, S3, CloudWatch, GuardDuty, KMS), GCP / Azure fundamentals |
| **Containers & Orchestration** | Docker, Kubernetes (K8s, EKS, Minikube), Helm Charts, Kustomize |
| **CI/CD & GitOps** | GitHub Actions, Jenkins, GitLab CI, ArgoCD, Flux |
| **Infrastructure as Code (IaC)** | Terraform, Ansible, AWS CloudFormation |
| **Static Application Security (SAST)** | SonarQube, Semgrep, Checkmarx |
| **Software Composition Analysis (SCA)**| Trivy, Snyk, OWASP Dependency-Check |
| **Container & OS Vulnerability** | Trivy, Grype, Docker Scout, Clair |
| **IaC Security & Compliance** | Checkov, tfsec, Terrascan, Kube-bench, OPA (Open Policy Agent) |
| **Dynamic Security Testing (DAST)** | OWASP ZAP, Nikto |
| **Secrets & Identity Management** | HashiCorp Vault, Gitleaks, TruffleHog, AWS Secrets Manager |
| **Runtime Security & Monitoring** | Falco, Prometheus, Grafana, ELK Stack, AWS CloudWatch |
| **Scripting & Automation** | Bash / Shell Scripting, Python, YAML, Groovy |

---

## 🚀 Featured DevSecOps Projects

### 1. 🛡️ Enterprise Automated DevSecOps Pipeline
- **Overview:** Implemented a full multi-stage CI/CD pipeline using **GitHub Actions** and **AWS EKS** enforcing automated security gates at every commit.
- **Key Features:**
  - Integrated **Gitleaks** to prevent secret leakage in commits.
  - Automated code analysis via **SonarQube** with quality gate thresholds.
  - Container scanning using **Trivy** that blocks build upon detection of CRITICAL/HIGH CVEs.
  - Post-deployment DAST scanning with **OWASP ZAP**.
- **Tech Stack:** `GitHub Actions`, `Docker`, `SonarQube`, `Trivy`, `OWASP ZAP`, `AWS EKS`, `ArgoCD`.
- **Repository:** [View Code & Pipeline](https://github.com/singhatulanand33/devsecops-portfolio)

---

### 2. ☸️ Zero-Trust Kubernetes Security & Policy Hardening
- **Overview:** Secured a production-grade Kubernetes cluster implementing Zero-Trust network policies, admission controllers, and runtime threat detection.
- **Key Features:**
  - Enforced admission control policies with **OPA Gatekeeper** and **Kyverno** (disallowing root containers, enforcing read-only root filesystems).
  - Deployed **Falco** for behavioral runtime monitoring and alerting to Slack upon unexpected shell executions.
  - Automated CIS Benchmark audits via **kube-bench** and **kube-hunter**.
- **Tech Stack:** `Kubernetes`, `OPA Gatekeeper`, `Falco`, `Kyverno`, `Calico CNI`, `Helm`.

---

### 3. 📜 Compliant Infrastructure as Code (IaC) with Terraform
- **Overview:** Designed modular, production-ready AWS cloud infrastructure automated via Terraform with pre-deployment security linting.
- **Key Features:**
  - Integrated **Checkov** and **tfsec** into pull request checks to prevent security misconfigurations (open S3 buckets, permissive security groups).
  - Implemented automated state management with S3 remote backend and DynamoDB locking.
- **Tech Stack:** `Terraform`, `AWS (VPC, IAM, EKS, RDS)`, `Checkov`, `tfsec`, `GitHub Actions`.

---

### 4. 🔑 Centralized Secrets Management with HashiCorp Vault
- **Overview:** Deployed and configured HashiCorp Vault for dynamic secrets generation and zero-trust credential distribution for microservices.
- **Key Features:**
  - Replaced hardcoded credentials with dynamic, short-lived AWS IAM and database credentials.
  - Integrated Vault Agent Sidecar injector for seamless Kubernetes pod secret injection.
- **Tech Stack:** `HashiCorp Vault`, `Kubernetes`, `AWS KMS`, `Consul`, `Docker`.

---

## 📈 GitHub Analytics & Activity

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=singhatulanand33&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="Atul's GitHub Stats" width="48%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=singhatulanand33&theme=tokyonight&hide_border=true" alt="Atul's Streak Stats" width="48%" />
</div>

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=singhatulanand33&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" />
</div>

---

## 📜 Certifications & Continuous Learning
- 🎖️ **AWS Certified Solutions Architect** *(In Progress / Completed)*
- 🎖️ **Certified Kubernetes Administrator (CKA)** / **CKS** *(Security Focus)*
- 🎖️ **HashiCorp Certified: Terraform Associate**

---

## 📬 Connect With Me

<p align="center">
  <a href="https://github.com/singhatulanand33"><img src="https://img.shields.io/badge/GitHub-singhatulanand33-181717?style=flat-square&logo=github" /></a>
  <a href="https://linkedin.com/in/"><img src="https://img.shields.io/badge/LinkedIn-Atul%20Anand%20Singh-0077B5?style=flat-square&logo=linkedin" /></a>
  <a href="mailto:singh.atulanand33@gmail.com"><img src="https://img.shields.io/badge/Email-singh.atulanand33%40gmail.com-D14836?style=flat-square&logo=gmail" /></a>
</p>

<div align="center">
  <i>⭐ Feel free to star this repository if you find it helpful! ⭐</i>
</div>
