<div align="center">

# ISMS Implementation Case Study — ISO/IEC 27001:2022

### Digital Al-Afaq Bank — Phase 1: Digital Banking Security

***A complete governance, risk and compliance (GRC) documentation set for an Information Security Management System (ISMS) aligned with ISO/IEC 27001:2022***

![Standard](https://img.shields.io/badge/Standard-ISO%2FIEC%2027001%3A2022-0B2545)
![Domain](https://img.shields.io/badge/Domain-ISMS%20%2F%20GRC-1282A2)
![Scope](https://img.shields.io/badge/Scope-Phase%201%20Digital%20Banking-0E7C7B)
![Status](https://img.shields.io/badge/Status-Pre--Certification%20Baseline-F4A259)
![Type](https://img.shields.io/badge/Type-Educational%20Case%20Study-6A4C93)

</div>

---

## ⚠️ Disclaimer

> **This is a fictional, educational case study.** Digital Al-Afaq Bank is an imaginary organization created solely for an academic graduation project. All names, incidents, risks, budgets, dates and figures are fabricated for learning purposes and do not represent any real institution. No real customer, employee or organizational data is included.

---

## 📖 Overview

This repository documents the design of a full **Information Security Management System (ISMS)** for a fictional Saudi bank, built against **ISO/IEC 27001:2022** and informed by **SAMA** cybersecurity expectations and the **PDPL** (Saudi Personal Data Protection Law, SDAIA).

**Phase 1 Scope:** securing the bank's digital banking channels — **Afaq Plus** (mobile app) and **Afaq Net** (internet banking) — together with their supporting infrastructure, Riyadh primary data center, Security Operations Center (SOC), Jeddah disaster recovery site, and related cloud (AWS) and third-party dependencies.

The documentation follows the **Plan → Do → Check → Act (PDCA)** lifecycle and covers everything from organizational context and scope definition to internal audit and performance evaluation.

### Project at a Glance

| Metric | Value |
|---|---|
| In-scope assets | **117** assets across 7 categories |
| Assessed risks | **20** (10 asset-based + 10 scenario-based) |
| Highest risk scores | **20** — SQL Injection & Credential Theft |
| Annex A controls in SoA | **93** (all applicable) |
| Performance KPIs | **24** RAG-tracked measures |
| Internal audit result | **1 minor NC** (Clause 6.2), 0 major NC |
| Security budget context | SAR 12M → SAR 18M post-implementation |

---

## 🗂️ Project Structure

```
isms-iso27001-case-study/
├── 01-context-and-scope/            # Organizational context, interested parties, scope & exclusions
├── 02-governance-and-policies/      # Top-level policy + acceptable use (Clauses 5, A.5.1, A.5.10)
├── 03-objectives/                   # Measurable security objectives (Clause 6.2)
├── 04-risk-management/              # Methodology, asset inventory, asset-based register, RA report
├── 05-statement-of-applicability/   # SoA — 93 Annex A controls (Clause 6.1.3)
├── 06-operations-and-controls/      # Operating procedures + firewall configuration baseline
├── 07-incident-and-continuity/      # Incident response procedure + BCP/DR plan
└── 08-check-and-act/                # Internal audit report + ISMS performance report
```

### Document Map

| # | Document | ISO/IEC 27001 Focus | Purpose |
|---|---|---|---|
| 01 | Information Security Context, Requirements & Scope | Clause 4 | Organizational context, issues, interested parties, Phase 1 scope |
| 02 | Information Security Policy | Clause 5 | Top-level policy and governance framework |
| 03 | Asset-Based Risk Assessment (Excel) | Clauses 6.1.2 / 8.2 | 10 asset-based risks: scoring, treatment, post-treatment |
| 04 | Statement of Applicability (Excel) | Clause 6.1.3 | Applicability, justification, status and ownership of 93 controls |
| 05 | Risk Assessment & Treatment Methodology | Clause 6.1 | 5×5 risk matrix, acceptance criteria, treatment options |
| 06 | Information Security Objectives | Clause 6.2 | 5 objective groups with KRs, owners and quarterly timeline |
| 07 | Risk Assessment Report | Clauses 6.1 / 8.2 | Formal risk results submitted for top-management sign-off |
| 08 | Inventory of Assets (Excel) | A.5.9 | 117 classified assets with owners, CIA attributes and IDs |
| 09 | Acceptable Use Policy | A.5.10 | User-facing rules for secure use of assets |
| 10 | Incident Response Procedure | A.5.24–A.5.28 | Detection → triage → IRT → containment → recovery → lessons |
| 11 | Internal Audit Report | Clause 9.2 | Audit of Clauses 4–6; one minor NC + two observations |
| 12 | Security Operating Procedures (IT) | Clause 8.1 / A.8.x | Five operational steps securing digital channels |
| 13 | ISMS Performance Report | Clause 9.1 | 24 KPIs with RAG status tracking |
| 14 | Security Configurations Baseline (Excel) | A.8.9 | Palo Alto firewall baseline with verification evidence |
| 15 | BCP & Disaster Recovery Plan | A.5.29 / A.5.30 | BIA, RTO/RPO objectives, activation criteria, test schedule |

---

## 🔄 ISMS Workflow

```
Context & Scope      Governance      Objectives & Assets      Risk Assessment
    (Doc 01)    →     (Doc 02)    →      (Doc 06 + 08)     →   (Doc 05 → 03 → 07)
                                                            ↓
Audit & Performance ←   Controls & Operations    ←   Statement of Applicability
 (Docs 11 + 13)         (Docs 09, 12, 14)                  (Doc 04)
    │   → Incident Response (Doc 10) → Business Continuity & DR (Doc 15) → Continual Improvement
```

---

## 🎯 Key Highlights

- **Risk-based Phase 1 scope** — digital channels prioritized; branches, ATMs and full core-banking systems excluded with justified controlled dependencies.
- **Evidence-driven risk register** — every risk carries likelihood/impact scoring, Annex A mapping, treatment action, owner, and post-treatment residual level (7 High → 0 High after planned treatment).
- **Traceability by design** — unique asset IDs (IA-xxx, SW-xxx, HW-xxx) link the inventory to risks, controls, baselines, incidents and performance KPIs.
- **Hardest incidents turned into controls** — a 3-hour firewall misconfiguration outage, an unencrypted laptop loss, and phishing results directly shaped the treatment plan.
- **Honest readiness snapshot** — internal audit (1 minor NC on objectives planning) and a 24-KPI RAG dashboard show exactly where maturity stands before certification.

---

## 🎓 Intended Use

Academic and training purposes: GRC students, ISMS practitioners, and anyone studying how ISO/IEC 27001:2022 documentation fits together as one integrated system — from scope definition to continual improvement.

## 📄 License

Released for educational use. See [LICENSE](LICENSE).
