# PH Impact Sectors  
*A living reference for civic technology priorities in the Philippines.*

---

## 🇵🇭 Vision  
To empower **LGUs, civic organizations, and citizen innovators** to co-create digital public goods that improve service delivery, transparency, and trust — beginning with municipal pilots and expanding sector by sector.

---

## 🌐 Core Principles
- **Open by Default** – All code, docs, and data (non-PII) are open-licensed for replication.  
- **Privacy & Safety First** – No personal data unless explicitly authorized.  
- **Local First** – Design for offline or low-bandwidth environments.  
- **Iterative Pilots** – Launch fast, learn fast.  
- **Measured Impact** – Each pilot defines 3 measurable outcomes (e.g. lead time, citizen satisfaction, adoption).

---

## 🏛️ Priority Sectors for 2025-2026

| Sector | Description | Pilot / Template Repo | Sample Use Cases | Key Metrics |
|:--|:--|:--|:--|:--|
| **Governance** | Barangay and municipal service tracking (permits, complaints, certificates). | [`sector-governance-template`](https://github.com/PH-CivicTech/sector-governance-template) | E-permits dashboard, ticket workflow, digital queue | Lead time ↓, SLA compliance ↑, citizen satisfaction ↑ |
| **Education** | School transparency, attendance, and digital learning tools for public schools. | *(planned)* | Teacher dashboards, student ID QR codes, local LMS connectors | Attendance accuracy ↑, report automation ↑ |
| **Health** | Barangay health center digitization and preventive health campaigns. | *(planned)* | e-Clinic visits, medicine stock tracker, immunization reminders | Visit coverage ↑, stock-outs ↓ |
| **Agriculture** | Small-farm registry and yield tracking to connect farmers with LGU programs. | *(planned)* | Farmer registry, subsidy logs, digital receipts | Program reach ↑, paperwork ↓ |
| **Disaster & Climate** | Rapid reporting and resource coordination during calamities. | *(planned)* | Damage maps, relief tracking, early warning alerts | Response time ↓, relief accuracy ↑ |
| **Citizen Feedback & Data Commons** | Anonymous surveys and open, synthetic datasets for civic research. | [`open-datasets`](https://github.com/PH-CivicTech/open-datasets) | Citizen report APIs, synthetic data playground | Data reuse ↑, privacy incidents = 0 |

---

## 🧩 Sector Architecture
Each sector follows a **3-layer pattern**:
1. **Core Services** → provided by `civic-core` (auth, RBAC, health, audit).
2. **Sector Template** → lightweight Express app scaffold with health/ticket endpoints.
3. **Pilot Repo** → localized deployment (config, translations, anonymized fixtures).

Example:  
```
civic-core/
└── sector-governance-template/
    └── pilot-albuera-governance-2025/
```

---

## 📈 Pilot Roadmap
**Q4 2025** – Albuera Governance 2025 (Barangay service tracking)  
**Q1 2026** – Education Pilot (public school digital records)  
**Q2 2026** – Health Pilot (Barangay e-Clinic)  
**Q3 2026** – Agriculture Pilot (Farmer registry + subsidy tracking)

---

## 🤝 How to Propose a New Sector
1. Fork [`playbook`](https://github.com/PH-CivicTech/playbook).  
2. Create an RFC under `/RFCs/`.  
3. Use the “Civic Impact Proposal” issue template.  
4. Define **sector**, **context**, **outcome**, and **metrics**.  
5. Submit a pull request tagged `status:needs-design`.

---

## 📬 Contact
- Org: [@PH-CivicTech](https://github.com/PH-CivicTech)  
- Email: civictech.ph@gmail.com  
- Pilot support: `/playbook/GOVERNANCE.md` → “Sector Leads” section
