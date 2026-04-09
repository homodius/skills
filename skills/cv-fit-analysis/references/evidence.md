# Platform PM & Developer-Facing Role Evidence

This file surfaces experience that is underrepresented in standard CV outputs but is directly evidenced in `exp_eleks_po` within `master_resume.yaml`. Read this file when analyzing platform PM, API product, SDK, developer tooling, or infrastructure-as-product roles.

---

## API Lifecycle Ownership

**Evidence:** External ingestion APIs exposed to client systems + internal cross-team APIs where multiple development teams are affected.

**What this covers:**
- Versioning strategy and backward compatibility decisions
- Breaking-change communication — identifying all affected parties, coordinating migration paths or parallel API endpoints
- API design input: helped developers make decisions about data structures, APIs, and algorithms aligned with business logic

**YAML location:** `exp_eleks_po.responsibilities_extra` (API lifecycle bullet) + `exp_eleks_po.responsibilities` ("Helped developers make decisions about data structures, APIs, and algorithms")

**Framing note:** Present as "owned external and internal API surfaces including versioning decisions and breaking-change communication" — not just "worked with APIs."

---

## Developer-Facing Platform Surfaces

**Evidence:** Product includes a formal **"platform builder" role** and a **MongoDB pipeline editor** — a bespoke UI built for platform developers and configurators. This is explicitly a developer/configurator-facing product surface, not just an end-user feature.

**What this covers:**
- Developer tooling ownership (UI-heavy platform tooling, not CLI-only)
- Configurator-facing surfaces and their UX/product requirements
- Understanding of developer persona (configurators are internal developers)

**YAML location:** `exp_eleks_po.responsibilities_extra` (MongoDB pipeline editor / platform-builder bullet)

---

## RBAC / Permissions Model Ownership

**Evidence:** Led full user roles and permissions model redesign in 2024. Defined all new product roles, scoped RBAC permissions across the product, documented the access model — now serves as the team's reference architecture.

**What this covers:**
- Auth/access control product decisions (keys, tokens, permission scopes, RBAC)
- API credential and access management from a product design perspective

**YAML location:** `exp_eleks_po.responsibilities_extra` (RBAC bullet) + `exp_eleks_po.achievements` (RBAC achievement)

---

## Async Workload Product Design

**Evidence:** Core ingestion feature is fully async. Production workloads: spreadsheet files up to several GBs, 300+ columns, 500k+ rows. Owned all product decisions around status visibility, retry behavior, error handling, failure communication, and operational stability.

**What this covers:**
- Async/batch job patterns: queue management, status tracking, retry logic
- High-throughput file processing product requirements
- Operational reliability product thinking

**YAML location:** `exp_eleks_po.responsibilities_extra` (async ingestion bullet) + `exp_eleks_po.achievements` (async scale achievement)

---

## Compliance & Data Handling Decisions

**Evidence:** Product operates under:
- **FedRAMP-adjacent B2G constraints** — US government software compliance requirements
- **GDPR** — data handling for European contexts
- **Tenant isolation** — ~20% of the product surface is cross-tenant (cloud admin, sales portal, data links, tenant migration); all decisions in this area owned by candidate
- **Encrypted API payloads** — candidate made decisions about transmitting sensitive data encrypted and storing it in non-exposed form
- **Data retention & deletion** — defined policies; currently addressing gaps in retention lifecycle

**What this covers:**
- Data residency / sovereignty awareness (FedRAMP region constraints)
- Tenant isolation design (enterprise infrastructure product thinking)
- Compliance-constrained product delivery

**YAML location:** `exp_eleks_po.responsibilities_extra` (compliance/data handling bullet)

---

## MCP Developer Tooling — Full PM Ownership

**Evidence:** 3 MCP servers in production: `coras-kb` (semantic search), `coras-jira` (live Jira API), Zephyr Squad (43+ tools). Full PM ownership: roadmap, prioritization, scope, rollout. Entire team currently uses it (devs, QA, PMs).

**Success metrics in constrained environment:** B2G security prevents direct user analytics. Measured via customer satisfaction proxy + reduction in follow-up request/bug report volume. Some features are intentionally designed to "trip" users if they deviate — a deliberate quality gate in a no-direct-feedback environment.

**YAML location:** `exp_eleks_po.responsibilities_extra` (MCP ownership bullets) + `exp_eleks_po.achievements` (AI-SDLC achievement)

---

## AI Ecosystem Familiarity

**Evidence:** AWS AI Practitioner certification (Feb 2025–2028) — curriculum covers LangChain, LlamaIndex, model serving concepts, and AI ecosystem frameworks. Hands-on: AWS Bedrock, pgvector, Ollama, MCP.

**YAML location:** `certifications[0].scope_note`

---

## Developer Documentation Quality

**Evidence:** Sole documentation owner for a 50+ person project (Nemlig.com, ~500 VMs). Created ~100 dense technical pages covering system operations, infrastructure, APIs, and troubleshooting. Tested and documented 3rd-party API integrations using Postman — covering request/response flows, error handling, edge cases (payment provider API migration).

**YAML location:** `exp_eleks_info_dev` (Nemlig role)
