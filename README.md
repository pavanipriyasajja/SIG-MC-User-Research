# Multi-Cluster Kubernetes UX Research

## 📌 Purpose

This repository is dedicated to documenting our **user research efforts** aimed at understanding the challenges and needs of engineers working with **multi-cluster Kubernetes environments**.

As organizations scale their cloud infrastructure, managing multiple Kubernetes clusters has become a common but complex practice. Through this research initiative, we aim to build more intuitive, effective, and centralized multi-cluster user experiences. This research is not tied to a specific implementation or tool. Instead, it is focused on understanding the diverse realities of engineers, architects, and platform teams working across multi-cluster setups. 
<br>

Here is the project proposal doc link : https://docs.google.com/document/d/1uCyHpI5zV1ME9qBtGjLkrIhpl3iXe-zQsn0SSbBiAE4/edit?usp=sharing 

---
## ✅ Research Objectives

**1. Current State Analysis**
- Map typical observability architectures in multi-cluster environments (e.g., hub-and-spoke, federated monitoring, per-cluster observability).
- Understand how monitoring is bootstrapped and maintained over time (manual vs. automated, GitOps, Helm, etc.).

**2. Tooling Landscape**
- Identify the full stack of tools in use (metrics, logs, traces, dashboards, alerting, storage, etc.).
- Assess how these tools are hosted: self-managed vs. managed services (e.g., Grafana Cloud, Datadog, New Relic).
- Explore the level of integration or fragmentation across these tools.

**3. Operational Workflows**
- Understand how users:
Detect issues (alerting, dashboards, automated checks)
Investigate incidents (root cause analysis, logs/traces review)
Collaborate during outages or investigations (Slack, Notebooks, etc.)
- Map hand-offs between DevOps, SREs, developers, and platform teams.

**4. Cluster Federation & Data Aggregation**
- Investigate how users centralize data from multiple clusters (e.g., Thanos, Cortex, custom pipelines).
- Understand challenges related to cross-cluster query performance and data consistency.

**5. Performance and Reliability Concerns**
- Document issues around high cardinality, metric retention, scalability, and cost.
- Identify common bottlenecks or failures in observability pipelines.


**6. Security & Compliance**
- Understand how users manage access control (RBAC, multitenancy) in observability tooling.
- Explore compliance requirements for observability data (e.g., log redaction, retention policies).


**7. Customization & Extensibility**
- Learn how teams customize observability dashboards, alerting rules, or pipelines to suit their needs.
- Identify needs around automation or templating (e.g., Jsonnet, Grafonnet, Kustomize).

**8. User Experience & Frustration Points**
- Gather qualitative feedback on UX challenges:
Dashboard usability
Alert fatigue
Learning curves of different tools
- Evaluate ease of onboarding new team members to the observability stack.

**9. Desired Improvements**
- Explore what an “ideal” multi-cluster observability experience looks like.
- Identify missing capabilities users wish existed.
- Prioritize features that would save time, reduce complexity, or improve incident response.

**10. Maturity & Adoption Journey**
- Assess where organizations are in their observability journey (e.g., early-stage, scaling, mature).
- Identify key events or triggers that led teams to evolve from single-cluster to multi-cluster observability.

<br>
## 🎯 Project Golas

- Uncover User Challenges in Multi-Cluster Observability
 Identify real-world pain points, inefficiencies, and unmet needs in how users monitor and manage Kubernetes across multiple clusters.

- Validate Product and Platform Assumptions
 Ensure our observability strategy aligns with how users actually work, what they need, and what they’re struggling with.

- De-Risk Feature and Roadmap Decisions
 Use data-driven insights to prioritize the right features and avoid building tools that miss the mark.

- Gain Competitive Intelligence
 Understand the current tooling landscape, adoption trends, and where we can differentiate or integrate more effectively.

- Enable Scalable, User-Centered Design
 Build a foundation for solutions that support real user workflows at scale—across clusters, teams, and environments.

- Establish Authority and Influence in the Ecosystem
 Position our team as a thoughtful contributor to the Kubernetes observability space by openly sharing research-backed insights.


<br>
## 🎯 Target Audience
This research is aimed at professionals who operate, observe, and monitor Kubernetes clusters—especially those managing multi-cluster environments. We’re focused on roles and teams that are responsible for maintaining system health, performance, and reliability at scale.


**👥 Primary Audience**

**Site Reliability Engineers (SREs)**
Responsible for uptime, incident response, and observability pipelines
Often manage monitoring tools, alerting rules, and SLIs/SLOs

**Platform Engineers**
Build and maintain internal Kubernetes platforms and developer infrastructure
Standardize observability tooling across multiple clusters and teams

**DevOps Engineers / Infrastructure Engineers**
Automate infrastructure, CI/CD, and observability stacks
Handle deployment and maintenance of tools like Prometheus, Grafana, etc.

**Cloud Architects / Kubernetes Administrators**
Design and implement multi-cluster Kubernetes strategies
Evaluate trade-offs in observability tools and cross-cluster data aggregation
Developers with Operational Responsibilities (DevOps-minded teams)

**Own microservices and monitor service health**
Interact directly with dashboards, logs, alerts, and traces


**🎯 Secondary Audience**

**Engineering Managers / Tech Leads**
Oversee observability strategy, performance budgets, and team workflows.

**Security & Compliance Engineers**
 Interested in access control, audit logs, data retention, and multitenancy within observability systems.

**Tooling/Product Teams (Internal or External)**
 Building solutions that require observability integrations or are affected by monitoring infrastructure.


<br>
## 🔍 Scope of Research
The scope covers both what we’re studying and how we plan to collect insights.

✅ Research Methods (How We’ll Conduct the Study)
We will use a combination of qualitative and quantitative methods:

**User Interviews**
1:1 conversations (30–45 mins)
Deep-dive into workflows, tools, pain points, and decision-making
Conducted remotely over Zoom or Google Meet


**Surveys**
Short-form questionnaires to gather broad insights
Focused on tool usage, experience level, and common challenges
Helps validate and scale findings from interviews


**Usability Testing (if applicable in later stages)**
Test interaction with current or prototype observability setups
Identify friction points in dashboards, alerting workflows, and navigation

**Architecture Walkthroughs (Optional)**
Participants share anonymized diagrams or explain their setup
Helps visualize real-world implementations and tooling patterns

**Secondary Research**
Review of community discussions, GitHub issues, forums, and public architecture blogs for recurring themes

<br>

## 📌 Status of the Project
**Current Phase: 🟡 Planning**
We are currently in the planning phase of the research. This includes:

Finalizing research goals and objectives
Designing interview and survey questions
Identifying target participants and recruitment channels
Preparing consent and privacy documentation

✅ Next Step: Begin participant outreach and schedule user interviews.

Here is the survey questions form : https://forms.gle/MPqnd77qkFkngqby7 

<br>
<hr>
## Community, discussion, contribution, and support

Learn how to engage with the Kubernetes community on the [community page](http://kubernetes.io/community/).

You can reach the maintainers of this project at:

- [Slack](https://slack.k8s.io/)
- [Mailing List](https://groups.google.com/a/kubernetes.io/g/dev)

### Code of conduct

Participation in the Kubernetes community is governed by the [Kubernetes Code of Conduct](code-of-conduct.md).

[owners]: https://git.k8s.io/community/contributors/guide/owners.md
[Creative Commons 4.0]: https://git.k8s.io/website/LICENSE
