<p align="center">
  <img src="https://img.shields.io/badge/11%20stacks-4F6EF7?style=flat-square" alt="11 stacks" />
  <img src="https://img.shields.io/badge/100%25%20Azure%20Verified%20Modules-0078D4?style=flat-square" alt="100% AVM" />
  <img src="https://img.shields.io/badge/aligned%20with%2010%20frameworks-00D4A1?style=flat-square" alt="aligned with 10 frameworks" />
  <img src="https://img.shields.io/badge/MIT%20dev%20stacks-28a745?style=flat-square" alt="MIT-licensed dev stacks" />
</p>

## What is AethronOps?

Complete Terraform projects for Azure, ready to deploy. Built exclusively on [Azure Verified Modules (AVM)](https://azure.github.io/Azure-Verified-Modules/) — Microsoft's official Terraform modules.

No access to your Azure, your repo, or your credentials. You download the code. You own it.

---

### The hard part we solve

Writing a single Azure resource is easy. **Wiring 40–60 resources together** is where teams lose weeks: Private Endpoints, Diagnostic Settings, RBAC, NSG rules, Key Vault access, EventGrid alerts, FinOps automation, brownfield wiring to a shared platform... AethronOps generates all of it — end-to-end — then validates it with `terraform plan` + `checkov`.

---

### 11 stacks · 2 modes

| Stack | Workload | Database |
|---|---|---|
| platform-baseline | Shared foundation (VNet, NAT, NSG, DNS, Redis, KV) | — |
| app-service-postgresql | App Service | PostgreSQL Flexible Server |
| app-service-sql | App Service | Azure SQL Database |
| app-service-cosmosdb | App Service | Cosmos DB (NoSQL) |
| app-service-mysql | App Service | MySQL Flexible Server |
| app-service-mongodb | App Service | Azure DocumentDB (MongoDB vCore) |
| container-apps-postgresql | Container Apps | PostgreSQL Flexible Server |
| container-apps-sql | Container Apps | Azure SQL Database |
| container-apps-cosmosdb | Container Apps | Cosmos DB (NoSQL) |
| container-apps-mysql | Container Apps | MySQL Flexible Server |
| container-apps-mongodb | Container Apps | Azure DocumentDB (MongoDB vCore) |

**Two modes** per stack:
- **Dev** — minimal, public access, MIT-licensed, free. Available open-source in [aethronops/stacks](https://github.com/Aethronops/aethronops/tree/main/stacks).
- **Production** — VNet isolation, Private Endpoints, brownfield-ready, framework-aligned. Sold at [aethronops.com](https://aethronops.com).

---

### Aligned with industry frameworks

Every production stack ships with a `SECURITY-POSTURE.md` documenting which technical controls cover each framework. As of today the file references: **MCSB · CAF · WAF · GDPR/RGPD · NIS2 · DORA · CIS · ISO 27001 · SOC 2 · PCI-DSS**.

> These mappings are audit preparation aids. AethronOps stacks are **aligned with** these industry frameworks — they are not a certification, audit report, or compliance guarantee. Regulatory compliance always depends on your global context (organisational, processes, other systems).

---

### Pricing

| Plan | Price | What you get |
|------|------:|-------------|
| **Dev (open source)** | 0 € | 10 dev stacks, MIT licensed, public access. No account needed. |
| **Single** | 199 € HT | 1 production stack of your choice. Lifetime use within your organisation. |
| **All-Access** | 499 € HT | All 11 production stacks. Lifetime use within your organisation. |

One-time payment. No subscription. Source code delivered as ZIPs.

---

<p align="center">
  <a href="https://aethronops.com/stacks/"><strong>Browse the catalog →</strong></a>&nbsp;&nbsp;·&nbsp;&nbsp;<a href="https://aethronops.com">aethronops.com</a>&nbsp;&nbsp;·&nbsp;&nbsp;<a href="https://aethronops.com/contact/">Contact</a>
</p>
