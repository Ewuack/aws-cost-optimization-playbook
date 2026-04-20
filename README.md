# AWS Cost Optimization Playbook

**A Cloud TPM's strategic framework for reducing AWS infrastructure spend while maintaining performance, reliability, and compliance.**

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?style=flat-square&logo=amazonaws)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)
![Role](https://img.shields.io/badge/Role-Cloud%20TPM-blue?style=flat-square)

---

## Project Overview

This playbook documents a structured, cross-functional cost optimization program across five AWS infrastructure domains. It reflects real-world TPM leadership in identifying waste, aligning engineering and finance stakeholders, and delivering measurable savings without compromising system reliability.

**Business Context:** Enterprise cloud spend was growing 28% YoY with limited visibility into cost drivers. This playbook established the governance framework, optimization strategies, and monitoring dashboards that reduced annual infrastructure costs by 32%.

---

## Repository Structure

aws-cost-optimization-playbook/
|-- compute/           # EC2 rightsizing, Reserved Instance strategy, Spot Fleet policies
|-- storage/           # S3 lifecycle policies, EBS optimization, data tiering
|-- networking/        # NAT Gateway consolidation, data transfer optimization
|-- autoscaling/       # Auto Scaling policies, target tracking, scheduled scaling
|-- dashboards/        # CloudWatch + Cost Explorer dashboard configurations
|-- README.md

---

## Key Outcomes

| Metric | Before | After | Impact |
|--------|--------|-------|--------|
| Monthly AWS Spend | $186K | $127K | **-32% reduction** |
| Idle/Unused Resources | 23% of fleet | Under 3% | **Eliminated waste** |
| RI/SP Coverage | 18% | 72% | **Optimized commitments** |
| Cost Anomaly Detection | Manual/monthly | Automated/real-time | **Proactive governance** |

---

## Domain Breakdown

### `/compute` — EC2 Rightsizing & Commitment Strategy
- Instance family migration analysis (m5 to m6i, c5 to c6g Graviton)
- Reserved Instance vs. Savings Plan comparison model
- Spot Fleet integration for non-production workloads
- Rightsizing recommendations based on 30-day CloudWatch utilization data

### `/storage` — S3 & EBS Optimization
- S3 Intelligent-Tiering and lifecycle policy configurations
- EBS volume type migration (gp2 to gp3) with cost-performance analysis
- Snapshot retention and cleanup automation
- Cross-region replication cost assessment

### `/networking` — Data Transfer & NAT Optimization
- NAT Gateway consolidation across VPCs (6 to 2)
- VPC Endpoint implementation to reduce data transfer costs
- CloudFront distribution optimization for egress reduction

### `/autoscaling` — Dynamic Scaling Policies
- Target tracking policies calibrated to business-hour traffic patterns
- Scheduled scaling for predictable workload spikes
- Scale-in protection rules for stateful services
- Warm pool configuration for launch time optimization

### `/dashboards` — Cost Visibility & Monitoring
- CloudWatch dashboards for real-time spend tracking by team/service
- Cost Explorer saved reports and anomaly detection alerts
- Budget alerts with SNS notification integration
- Monthly cost allocation tag compliance reports

---

## Tools & Services

| Category | Tools |
|----------|-------|
| **AWS Services** | EC2, S3, EBS, CloudWatch, Cost Explorer, Auto Scaling, VPC, CloudFront |
| **Cost Management** | AWS Budgets, Savings Plans, Reserved Instances, Cost Allocation Tags |
| **Monitoring** | CloudWatch Dashboards, SNS, Cost Anomaly Detection |
| **Program Management** | Jira, Confluence, Datadog |

---

## TPM Lens — Program Management Perspective

This project demonstrates core Cloud TPM competencies:

- **Stakeholder Alignment:** Led cross-functional working group (Engineering, Finance, DevOps) with biweekly cost review cadence
- **Data-Driven Decisions:** Built executive dashboards translating technical metrics into business impact ($59K/month savings)
- **Risk Management:** Balanced cost reduction against reliability SLAs — zero availability regressions during optimization
- **Governance & Process:** Established tagging standards, cost approval workflows, and optimization runbook for ongoing compliance
- **Roadmap Execution:** Phased 12-week rollout with clear milestones, dependency mapping, and weekly status reporting

---

## Related Projects

| Project | Description |
|---------|-------------|
| [Cloud Migration Architecture](https://github.com/Ewuack/cloud-migration-architecture) | On-prem to AWS migration program |
| [HIPAA Cloud Governance Framework](https://github.com/Ewuack/hipaa-cloud-governance-framework) | Compliance-as-code for regulated environments |
| [Cloud Incident Response Simulation](https://github.com/Ewuack/cloud-incident-response-simulation) | Security incident detection and response |
| [Cloud SDLC Pipeline](https://github.com/Ewuack/cloud-sdlc-pipeline) | CI/CD pipeline with security gates |

---

**Author:** Erick Guacamaya — Cloud Technical Program Manager
**LinkedIn:** [linkedin.com/in/erickguacamaya](https://linkedin.com/in/erickguacamaya) | **GitHub:** [github.com/Ewuack](https://github.com/Ewuack)
