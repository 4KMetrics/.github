# 4KM

## Fix how you ship!

AI-powered insights to measure, diagnose, and fix your software delivery pipeline.

---

## How We Work

We embed with your team — assess your current delivery process, find the bottleneck, and fix it. No generic playbooks. Real infrastructure work, measured by the metrics that matter.

**Measure** → Baseline your DORA metrics to see where you actually stand

**Diagnose** → Pinpoint what's slowing you down — CI? Environments? Config drift? Release process?

**Fix** → Implement the infrastructure changes with your team

**Prove** → Show the before/after with hard numbers

---

## The 4 Key Metrics

| Metric | What It Tells You | Elite Target |
|--------|-------------------|--------------|
| **Deployment Frequency** | How often you ship | On-demand |
| **Lead Time for Changes** | Commit to production | < 1 hour |
| **Change Failure Rate** | How often deploys break things | < 5% |
| **Time to Restore** | How fast you recover | < 30 min |

*Based on DORA research — the metrics that separate elite performers from everyone else.*

---

## What We Deliver
```mermaid
flowchart LR
    subgraph YOUR_TEAM["Your Engineers Own"]
        A[Code] --> B[Build] --> C[Test]
    end

    subgraph 4KM_HANDLES["4KM Handles"]
        D[Security Scan] --> E[Package]
        E --> F[Deploy Dev]
        F --> G[Validate]
        G --> H[Promote Staging]
        H --> I[Perf Test]
        I --> J[Security Test]
        J --> K[Deploy Prod]
        K --> L[Observe]
        L --> M[Respond]
    end

    C --> D

    style YOUR_TEAM fill:#e1f5fe
    style 4KM_HANDLES fill:#fff3e0
```

Your engineers focus on code, architecture, and the problems only humans can solve. We handle everything between commit and production — and everything after.

| Capability | What You Get |
|------------|--------------|
| **CI/CD Pipelines** | GitHub Actions, GitLab CI — fast, reliable, maintained |
| **Infrastructure** | Terraform modules for AWS, GCP, Azure |
| **Kubernetes** | Production-grade clusters, RBAC, autoscaling, security |
| **Observability** | Prometheus, Grafana, OpenTelemetry — see everything |
| **Security** | SAST, DAST, dependency scanning baked into the pipeline |
| **ML Deployment** | SageMaker endpoints, inference pipelines |

---

## The Full Pipeline
```mermaid
flowchart TB
    subgraph DEV["Development"]
        CODE[Code & Commit]
        PR[Pull Request]
        REVIEW[AI-Assisted Review]
    end

    subgraph DEVOPS["DevOps"]
        CI[CI Pipeline]
        CD[CD Pipeline]
        IaC[Terraform / IaC]
        GUARD[Guardrails & Gates]
    end

    subgraph PROD["Production"]
        DEPLOY[Deployment]
        OBS[Observability]
        FEEDBACK[Feedback Loop]
    end

    CODE --> PR --> REVIEW --> CI
    CI --> GUARD --> CD --> IaC --> DEPLOY
    DEPLOY --> OBS --> FEEDBACK --> CODE

    style DEV fill:#e1f5fe
    style DEVOPS fill:#fff3e0
    style PROD fill:#fce4ec
```

---

## Why 4KM

| | |
|---|---|
| **Domain depth** | Years of hands-on DevOps — not generic consulting from a textbook |
| **Partnership** | We embed with your team, building trust and context over time |
| **Speed** | 2-week delivery cycles — ship, measure, iterate |
| **Durability** | Battle-tested patterns that survive platform shifts and hype cycles |
| **Pragmatism** | Open-source tools and community modules — no custom bloat |