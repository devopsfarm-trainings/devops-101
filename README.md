# DevOps 101 — Overview of DevOps Practices

## What is DevOps?

DevOps is a culture and set of practices that brings **Development** and **Operations** teams together to deliver software faster, more reliably, and at scale.

Before DevOps, developers wrote code and threw it over the wall to ops. Ops deployed it and prayed. DevOps tears down that wall.

> **Core idea:** Build it, ship it, run it — same team, same responsibility.

---

## The DevOps Lifecycle

```
Plan → Code → Build → Test → Release → Deploy → Operate → Monitor → (back to Plan)
```

Every loop of this cycle is a chance to ship value and learn from production.

---

## Key Practices

### 1. Version Control
Everything as code — application code, infrastructure, configs, scripts.
- Tool: **Git** (GitHub / GitLab / Bitbucket)
- Rule: if it's not in Git, it doesn't exist

### 2. CI/CD — Continuous Integration & Continuous Delivery
Automate the path from code commit to production.
- **CI:** every push triggers automated build + test
- **CD:** every passing build is deployable (or auto-deployed)
- Tools: Jenkins, GitHub Actions, GitLab CI, ArgoCD

### 3. Infrastructure as Code (IaC)
Provision servers, networks, and cloud resources using code — not click-ops.
- Tools: **Terraform**, Ansible, CloudFormation
- Benefit: repeatable, reviewable, version-controlled infra

### 4. Containerisation & Orchestration
Package apps and their dependencies into containers. Run them at scale.
- **Docker** — build and run containers
- **Kubernetes** — orchestrate containers across clusters

### 5. Monitoring & Observability
You can't fix what you can't see.
- **Metrics:** Prometheus, Grafana
- **Logs:** ELK Stack, Loki
- **Traces:** Jaeger, OpenTelemetry
- Key signals: Latency, Traffic, Errors, Saturation (the **RED / USE / Four Golden Signals** methods)

### 6. Site Reliability Engineering (SRE)
Google's approach to running production systems reliably.
- Define **SLOs** (what "reliable" means)
- Track **error budgets** (how much can break before users notice)
- Build for failure — chaos engineering, runbooks, on-call

### 7. Security (DevSecOps)
Shift security left — build it into the pipeline, not bolt it on at the end.
- Static code analysis, dependency scanning, container image scanning
- Tools: Trivy, Snyk, SonarQube

---

## Core Principles

| Principle | What it means |
|---|---|
| **Automate everything** | Manual = slow, error-prone, not scalable |
| **Fail fast** | Catch bugs early in CI, not in production |
| **Small, frequent releases** | Less risk than big-bang deployments |
| **Feedback loops** | Monitoring → learning → improving |
| **Shared ownership** | Dev and Ops both own production |
| **Everything as code** | Infra, config, pipelines — all in Git |

---

## DevOps Toolchain at a Glance

```
Source Control    →  Git, GitHub, GitLab
CI/CD             →  Jenkins, GitHub Actions, ArgoCD
Containers        →  Docker, Podman
Orchestration     →  Kubernetes (EKS, GKE, AKS)
IaC               →  Terraform, Ansible
Monitoring        →  Prometheus, Grafana, Loki
Security          →  Trivy, Snyk, SonarQube
Cloud             →  AWS, Azure, GCP
```

---

## DevOps vs Traditional IT

| | Traditional | DevOps |
|---|---|---|
| Release cycle | Months | Days / hours |
| Deployment | Manual | Automated |
| Infra changes | Tickets | Code PRs |
| Incident response | Reactive | Proactive (alerts) |
| Team structure | Silos | Shared ownership |

---

## Common Misconceptions

**"DevOps is just a job title."**
No — it's a culture. Tools without the culture don't work.

**"DevOps means no Ops team."**
No — it means Dev and Ops collaborate closely, not that one replaces the other.

**"You need to learn every tool."**
No — understand the concepts first. Tools change, principles don't.

---

## Where This Course Takes You

```
DevOps 101 (this doc)
    ↓
Month 1 — Linux, Git, Python, Docker
    ↓
Month 2 — Kubernetes, Terraform, Ansible, CI/CD
    ↓
Month 3 — SRE, Observability, DevSecOps
    ↓
Month 4 — GenAI + Capstone Project
```

---

*Part of the DevOpsFarm curriculum — [training.devopsfarm.in](https://training.devopsfarm.in)*
