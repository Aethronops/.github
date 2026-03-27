![Header](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,12&height=280&section=header&text=%C3%86thronOps&fontSize=60&fontColor=ffffff&animation=fadeIn&desc=Azure%20infrastructure%20production-ready%20in%201%20click&descSize=18&descAlignY=72)

<p align="center">
  <img src="https://img.shields.io/badge/78%20stacks-4F6EF7?style=flat-square" alt="78 stacks" />
  <img src="https://img.shields.io/badge/7%20frameworks-00D4A1?style=flat-square" alt="7 frameworks" />
  <img src="https://img.shields.io/badge/100%25%20Azure%20Verified%20Modules-0078D4?style=flat-square" alt="100% AVM" />
  <img src="https://img.shields.io/badge/83%2F83%20plan%20%2B%20checkov%20pass-28a745?style=flat-square" alt="83/83 validated" />
  <img src="https://img.shields.io/badge/43%2B%20real%20Azure%20deploys-ff6600?style=flat-square" alt="43+ deploys" />
</p>

> **Important:** AethronOps generates Terraform code aligned with Azure security best practices. The included compliance mappings (SECURITY-POSTURE.md) are provided as audit preparation aids only. They do not constitute compliance certification, legal advice, or guarantee of regulatory conformity. You are solely responsible for validating compliance in your own environment.

---

## What is AethronOps?

Complete Terraform projects for Azure, ready to deploy. No access to your Azure, your repo, or your credentials. You download the code. You own it.

Built exclusively on [Azure Verified Modules (AVM)](https://azure.github.io/Azure-Verified-Modules/) -- Microsoft's official Terraform modules.

---

## The hard part we solve

Writing a single Azure resource is easy. **Wiring 40-100 resources together** is where teams lose weeks:

- Private Endpoints pointed at the right subnet with the right DNS zone
- Diagnostic Settings forwarding every resource to Log Analytics
- RBAC assignments between Managed Identities and each service
- Network rules, NSG configurations, Key Vault access policies
- Budget alerts, auto-shutdown, storage lifecycle in FinOps

AethronOps generates all of that wiring -- end-to-end -- then validates it:

- **83/83** premium stacks pass `terraform validate` + `terraform plan` + `checkov` (0 failed)
- **43+** stacks deployed and destroyed on real Azure (`terraform apply` verified)
- **12 to 107** Terraform resources per stack, all connected

---

## What you get in every stack

```
15-20 structured .tf files (CAF naming convention)
Every resource wired: networking, identity, monitoring, secrets, security
Private Endpoints, Managed Identity, TLS 1.2+, Key Vault
Log Analytics + App Insights + diagnostic settings on every resource
SECURITY-POSTURE.md: controls mapped to 7 frameworks
finops.tf: budget alerts, auto-shutdown, lifecycle policies
.checkov.yaml: documented justification for every skip
README.md: architecture overview + 3-step deployment guide
3 tiers: basic/ standard/ premium/ -- pick your security level
```

---

## 78 Stacks -- 5 Free

### Free stacks (no account needed)

| Stack | What it deploys |
|-------|----------------|
| **Governance Organization** | Management Groups, Azure Policy initiatives, centralized monitoring |
| **Governance Subscription** | Subscription-level Policy, RBAC, budgets, diagnostic settings |
| **Platform Management** | Log Analytics, Automation Account, Key Vault, monitoring baseline |
| **Storage Baseline** | Storage Account with Key Vault, network isolation, lifecycle rules |
| **Static Web App** | Azure Static Web App with Key Vault, Storage, Application Insights |

### Paid stacks (73)

| Category | Examples | Count |
|----------|---------|:-----:|
| Web Applications | App Service + PostgreSQL/MySQL/SQL/CosmosDB, API Gateway | 7 |
| Serverless | Function App variants, Serverless Full-Stack, Static Website | 6 |
| Container Apps | Container Apps + PostgreSQL/MySQL/SQL/CosmosDB | 5 |
| Kubernetes (AKS) | AKS Startup, Microservices, Platform, ACR, Artifact Registry | 5 |
| Databases | PostgreSQL, MySQL, SQL, CosmosDB, Redis, Storage | 5 |
| Database Admin | Monitoring packs for existing PG/MySQL/SQL/CosmosDB/Redis | 5 |
| IaaS VMs | VM Production, Dev Jump Box, VM+PostgreSQL/MySQL/SQL Server | 5 |
| AI and ML | OpenAI, RAG (5 variants), AI Foundry, MLOps, GenAI, Chatbot, Knowledge Hub | 14 |
| AI Cognitive | Vision, Speech, NLP, Document Intelligence, Knowledge Mining, Content Safety | 10 |
| Networking and Platform | Platform Connectivity, Multi-Region HA, Ops Management | 3 |
| Regulated Industries | FinTech PCI, Healthcare HDS, SaaS Multi-Tenant | 3 |
| Events | Event Streaming, Event-Driven Platform | 2 |

Each stack in **3 tiers**: `Basic` (dev/POC) -- `Standard` (production) -- `Premium` (enterprise, regulated)

---

## Frameworks mapped

![CAF](https://img.shields.io/badge/CAF-Cloud%20Adoption-0078D4?style=flat-square)
![WAF](https://img.shields.io/badge/WAF-5%20Pillars-0078D4?style=flat-square)
![MCSB](https://img.shields.io/badge/MCSB-v1-0078D4?style=flat-square)
![GDPR](https://img.shields.io/badge/GDPR-EU%202016%2F679-003399?style=flat-square)
![NIS2](https://img.shields.io/badge/NIS2-EU%202022%2F2555-003399?style=flat-square)
![DORA](https://img.shields.io/badge/DORA-EU%202022%2F2554-003399?style=flat-square)
![EU AI Act](https://img.shields.io/badge/EU%20AI%20Act-2024%2F1689-003399?style=flat-square)

DORA mappings apply to fintech stacks. EU AI Act mappings apply to AI stacks.

---

## Pricing

| Plan | Price | What you get |
|------|------:|-------------|
| Free | 0 EUR | 5 stacks (all 3 tiers) |
| Starter | 79 EUR | 1 stack of your choice (all 3 tiers) |
| Builder | 149 EUR | 5 stacks of your choice (all 3 tiers) |
| Architect | 249 EUR | All 78 stacks (all 3 tiers) |

---

[![Browse Stacks](https://img.shields.io/badge/Browse%20all%2078%20stacks-00D4A1?style=for-the-badge)](https://aethronops.com/stacks)
[![Website](https://img.shields.io/badge/aethronops.com-0A0A0F?style=for-the-badge&logo=googlechrome&logoColor=white)](https://aethronops.com)
[![Contact](https://img.shields.io/badge/contact%40aethronops.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:contact@aethronops.com)

**Built by** [@f-leroy](https://github.com/f-leroy) -- Microsoft Certified Trainer | Azure Solutions Architect Expert

![Footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,12&height=120&section=footer)
