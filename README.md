<div align="center">

# ⚡ Gangaram Dewasi
### **Platform Architect | DevOps & Cloud Architect | Enterprise GenAI & Agentic Systems**
**Bengaluru, India 🇮🇳**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gangaram-dewasi-/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GangaramD)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:gangaram136@gmail.com)
[![GCP Certified](https://img.shields.io/badge/GCP_Certified-Professional_Cloud_Architect-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)](https://cloud.google.com/certification)
[![Featured Repo](https://img.shields.io/badge/Featured_Repo-ai--systems-FF9900?style=for-the-badge&logo=amazondocumentdb&logoColor=white)](https://github.com/GangaramD/ai-systems)

<br/>

```text
🚀 Architecting Enterprise GenAI Platforms • AWS Bedrock AgentCore • Model Context Protocol (MCP)
☁️ Regulated Cloud Architecture • Immutable GitOps • Chaos Engineering & Resilience • FinOps
```

</div>

---

## 🎯 About Me & Engineering Focus

I am a **Platform Architect** with **9+ years of experience** designing and operating scalable cloud infrastructure, platform foundations, and enterprise GenAI agent systems across regulated financial environments and enterprise multi-client ecosystems.

- 🤖 **Enterprise AI & Agentic Platforms:** Architecting production GenAI systems with **Amazon Bedrock AgentCore** and the **Model Context Protocol (MCP)**, exposing enterprise tools and databases to **Claude Code**, **Cursor**, and internal portals with fine-grained authorization and prompt security.
- 🛡️ **Operational Resilience & Chaos Engineering:** Designing highly resilient cloud topologies, automated disaster recovery drills, and chaos engineering experiments with zero-downtime cross-region failovers.
- ⚙️ **GitOps & Platform Engineering:** Building immutable single-environment production pipelines, canary releases via **Argo CD**, infrastructure automation with **Terraform/Terragrunt**, and self-service internal developer platforms (IDPs).
- 🔐 **Zero-Trust Access & Governance:** Implementing serverless Just-In-Time (JIT) access platforms, fine-grained Cedar authorization policies, and automated audit telemetry.
- 📉 **Cloud FinOps:** Driving large-scale infrastructure right-sizing, container modernization (ECS Fargate/Kubernetes), and compute optimization.

---

## ⭐ Featured Project: AgentCore Gateway & MCP Architecture

### 🌐 [AgentCore Gateway & Reference Architecture (`ai-systems`)](https://github.com/GangaramD/ai-systems)
*Enterprise Model Context Protocol (MCP) Gateway on AWS: Governed, multi-target tool access for AI agents with decoupled inbound and outbound authentication.*

- **The Problem:** Hand-crafting tools inside individual agent apps causes credential sprawl, duplicated client plumbing, and zero centralized governance across LLM tool invocations.
- **The Solution:** A centralized tool adapter layer on AWS acting as a managed MCP server that converts heterogeneous backends (databases, microservices, SaaS) into standardized MCP tools (`tools/list` and `tools/call`).
- **Core Architectural Patterns:**
  - **Dynamic Zero-Tool Discovery:** Agents declare zero hardcoded tools, querying the Gateway endpoint at runtime to dynamically bind schemas to Claude Code, Cursor, or web frontends.
  - **Two-Legged Authentication Model:** Inbound caller identity (Amazon Cognito JWT) is decoupled from outbound target backend credentials (IAM Roles, 2LO API Keys, 3LO OAuth Tokens).
  - **Cedar Policy Evaluation:** Enforcing fine-grained tool authorization and prompt-injection mitigations before tool execution.
  - **Multi-Target Governed Adapters:** Securely routing tool requests to Aurora PostgreSQL (via RDS Data API), FastAPI microservices, GitHub, and enterprise knowledge bases.
- **Tech Stack:** `Amazon Bedrock` • `AgentCore` • `Model Context Protocol (MCP)` • `Terraform` • `Python 3.11+` • `FastAPI` • `Streamlit` • `Cognito` • `Aurora PostgreSQL`

👉 **View repository & documentation:** [github.com/GangaramD/ai-systems](https://github.com/GangaramD/ai-systems)

---

## 🏛️ Architecture & Platform Design Principles

Instead of fragile point-to-point integrations and ad-hoc infrastructure, my platform designs center around five fundamental architectural tenets:

1. **Governed Tool Access via Open Protocols:** Standardizing all agent-to-tool integrations through the Model Context Protocol (MCP), ensuring heterogeneous backends (databases, REST APIs, SaaS) are exposed through consistent, versioned contracts without leaking credentials into agent runtimes.
2. **Decoupled Identity & Zero-Trust Security:** Enforcing strict boundaries between inbound user/agent identity and outbound execution credentials. All invocations require authenticated bearer tokens, verified against fine-grained Cedar authorization policies with prompt-injection defenses.
3. **Paved-Road Platform Self-Service:** Empowering multidisciplinary teams through self-service internal developer platforms (IDPs) and golden paths, abstracting underlying infrastructure complexity while enforcing enterprise compliance by default.
4. **Immutable GitOps & Drift Elimination:** Treating Git as the single source of truth for both application and infrastructure states. Operating automated canary rollouts with Argo CD to eliminate environment drift and enable reliable, zero-downtime releases.
5. **Continuous Resilience & Chaos Validation:** Architecting systems with failure tolerance as a baseline. Validating cross-region failover and service impact tolerances through automated chaos engineering experiments (AWS FIS) and proactive telemetry.

---

## 🛠️ Technical Proficiencies & Tooling Matrix

<table>
  <tr>
    <td width="25%"><b>🧠 AI & Agentic Systems</b></td>
    <td>
      <img src="https://img.shields.io/badge/Amazon_Bedrock-FF9900?style=flat-square&logo=amazon-aws&logoColor=white" />
      <img src="https://img.shields.io/badge/Bedrock_AgentCore-FF9900?style=flat-square&logo=amazon-aws&logoColor=white" />
      <img src="https://img.shields.io/badge/Model_Context_Protocol-000000?style=flat-square&logo=anthropic&logoColor=white" />
      <img src="https://img.shields.io/badge/Strands_Agents-232F3E?style=flat-square&logo=amazon-aws&logoColor=white" />
      <img src="https://img.shields.io/badge/RAG_&_Knowledge_Bases-4169E1?style=flat-square&logo=databricks&logoColor=white" />
      <img src="https://img.shields.io/badge/Claude_Code-D97706?style=flat-square&logo=anthropic&logoColor=white" />
      <img src="https://img.shields.io/badge/Cursor_IDE-000000?style=flat-square&logo=visual-studio-code&logoColor=white" />
      <img src="https://img.shields.io/badge/Prompt_Injection_Mitigation-DC2626?style=flat-square&logo=auth0&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td width="25%"><b>☁️ Cloud & Compute</b></td>
    <td>
      <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white" />
      <img src="https://img.shields.io/badge/AWS_Lambda-FF9900?style=flat-square&logo=aws-lambda&logoColor=white" />
      <img src="https://img.shields.io/badge/ECS_Fargate-FF9900?style=flat-square&logo=amazon-aws&logoColor=white" />
      <img src="https://img.shields.io/badge/Amazon_EKS-FF9900?style=flat-square&logo=amazon-eks&logoColor=white" />
      <img src="https://img.shields.io/badge/AWS_Amplify-FF9900?style=flat-square&logo=aws-amplify&logoColor=white" />
      <img src="https://img.shields.io/badge/DynamoDB-4053D6?style=flat-square&logo=amazon-dynamodb&logoColor=white" />
      <img src="https://img.shields.io/badge/Aurora_PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white" />
      <img src="https://img.shields.io/badge/Azure_AKS-0089D6?style=flat-square&logo=microsoft-azure&logoColor=white" />
      <img src="https://img.shields.io/badge/Google_Cloud_GKE-4285F4?style=flat-square&logo=google-cloud&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td width="25%"><b>⚙️ Platform & GitOps</b></td>
    <td>
      <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white" />
      <img src="https://img.shields.io/badge/Terragrunt-5C4EE5?style=flat-square&logo=terraform&logoColor=white" />
      <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" />
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
      <img src="https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white" />
      <img src="https://img.shields.io/badge/Argo_CD-EF6C00?style=flat-square&logo=argo&logoColor=white" />
      <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white" />
      <img src="https://img.shields.io/badge/GitLab_CI-FC6D26?style=flat-square&logo=gitlab&logoColor=white" />
      <img src="https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td width="25%"><b>🛡️ Resilience, Security & FinOps</b></td>
    <td>
      <img src="https://img.shields.io/badge/Operational_Resilience-008080?style=flat-square&logo=shield&logoColor=white" />
      <img src="https://img.shields.io/badge/AWS_FIS_Chaos-FF9900?style=flat-square&logo=amazon-aws&logoColor=white" />
      <img src="https://img.shields.io/badge/BCP_&_Cross_Region_DR-0284C7?style=flat-square&logo=amazon-route53&logoColor=white" />
      <img src="https://img.shields.io/badge/Cedar_Authorization-3B82F6?style=flat-square&logo=auth0&logoColor=white" />
      <img src="https://img.shields.io/badge/Serverless_JIT_Access-10B981?style=flat-square&logo=shield&logoColor=white" />
      <img src="https://img.shields.io/badge/PCI--DSS_&_SOC_2-475569?style=flat-square&logo=securityscorecard&logoColor=white" />
      <img src="https://img.shields.io/badge/Cloud_FinOps-059669?style=flat-square&logo=google-cloud&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td width="25%"><b>📊 Observability & Data</b></td>
    <td>
      <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" />
      <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" />
      <img src="https://img.shields.io/badge/Thanos-008080?style=flat-square&logo=prometheus&logoColor=white" />
      <img src="https://img.shields.io/badge/CloudWatch-FF4F8B?style=flat-square&logo=amazon-cloudwatch&logoColor=white" />
      <img src="https://img.shields.io/badge/OpenSearch_ELK-005571?style=flat-square&logo=opensearch&logoColor=white" />
      <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apache-kafka&logoColor=white" />
      <img src="https://img.shields.io/badge/Apache_Flink-E6526F?style=flat-square&logo=apache-flink&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td width="25%"><b>💻 Languages & APIs</b></td>
    <td>
      <img src="https://img.shields.io/badge/Python_3.11+-3776AB?style=flat-square&logo=python&logoColor=white" />
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
      <img src="https://img.shields.io/badge/Bash_Shell-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white" />
      <img src="https://img.shields.io/badge/SQL_PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white" />
    </td>
  </tr>
</table>

---

## 📊 GitHub Analytics & Activity

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=GangaramD&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="Gangaram's GitHub Stats" height="165" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=GangaramD&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" height="165" />
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com/?user=GangaramD&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</div>

---

<div align="center">

### 🤝 Let's Connect

Looking to discuss **Enterprise GenAI Architectures**, **Model Context Protocol (MCP)**, **Cloud Resilience**, or **Platform Engineering**?

[![LinkedIn](https://img.shields.io/badge/LinkedIn-View_Full_Profile_&_Career_History-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gangaram-dewasi-/)
[![Email](https://img.shields.io/badge/Email-Get_in_Touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:gangaram136@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GangaramD)

<sub>*For detailed employment history, professional recommendations, and career milestones, visit my [LinkedIn profile](https://www.linkedin.com/in/gangaram-dewasi-/).*</sub>

</div>
