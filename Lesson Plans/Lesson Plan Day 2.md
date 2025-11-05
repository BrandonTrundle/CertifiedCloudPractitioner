# Lesson Plan — Day 2 (Staying in Domain 1)

> **Theme:** “Explain it, defend it, apply it.” No memorization drills without application.

## Logistics

- **Date:** Tomorrow
- **Scope:** Domain 1 (Tasks **1.2→1.4**) + integration back to **1.1**
- **Outputs:** short written explanations, mini-diagrams, a 1-page “teach-back,” and a scored capstone set.

---

## Learning Objectives (by the end of Day 2, you can…)

1. **WAF Mastery (1.2):**

   - State each pillar, **trade-offs** between pillars, and **2 service examples** per pillar.
   - Conduct a **Well-Architected Review** outline (inputs → findings → remediations).

2. **CAF & Migration (1.3):**

   - Match **CAF perspectives** to stakeholders & decisions.
   - Choose the right **6 R** for a scenario and justify it.
   - Pick **migration tooling** (Snowball/DataSync/DMS/Migration Hub) with a reason.

3. **Cloud Economics (1.4):**

   - Explain **fixed vs variable** costs; compute simple **TCO deltas**.
   - Distinguish **rightsizing** vs **auto scaling**.
   - Argue how **managed services** and **automation** lower total cost and risk.

---

## Schedule & Work Plan

### Block 1 — WAF Deep Application (75–90 min)

- **Drill A (Explainers):**
  For each pillar, write **3 bullets**:

  1. one-line definition in plain English,
  2. the **risk** it reduces,
  3. **2 AWS services** that operationalize it (e.g., **Security** → IAM/KMS; **OPEX** → CloudFormation/CodePipeline).

- **Drill B (Trade-offs):**
  6 mini-scenarios where two pillars conflict (e.g., **Reliability vs Cost**; **Security vs Performance**). For each, propose a **balanced decision**.
- **Drill C (WAR review skeleton):**
  Create a **Well-Architected Review** checklist: questions to ask, metrics to pull, outputs to deliver (findings/severity/remediation plan).

**Deliverable:** 1-page WAF matrix (Pillar → risks → services → metrics).

---

### Block 2 — CAF + Migration Strategy Mechanics (60–75 min)

- **Drill A (CAF mapping):**
  For each **CAF perspective** (Business, People, Governance, Platform, Security, Operations), write:

  - **Owner** (role), **Decisions**, **Artifacts** (e.g., Business → KPIs/ROI, People → training plan).

- **Drill B (6 R’s with tooling):**
  Build a table: **Workload** → **Chosen R** → **Reason** → **Migration tool(s)** (Snowball/DataSync/DMS/Application Migration Service) → **Risks** → **Mitigations**.
- **Drill C (Tool selection):**
  Given 6 short scenarios (data size, timeline, network limits, DB type), pick **one tool** and **1-sentence justification**.

**Deliverable:** CAF matrix + 6 R’s table with tool mapping.

---

### Block 3 — Cloud Economics (60–75 min)

- **Drill A (Explainers):**

  - Fixed vs variable costs → write the **money sentence** and one example each (on-prem HVAC vs S3 storage).
  - **Rightsizing vs Auto Scaling** → definition + example + KPI you’d watch (CPU, latency, QPS).

- **Drill B (Mini-TCO):**
  Given a tiny scenario (3 m5.large on-prem equivalents, 40% avg utilization, dev off-hours), compute **qualitative** cost improvements via:

  1. **right-size** to m6g.medium,
  2. **turn off after hours**,
  3. switch to a **managed DB** (ops cost removed).
     (No calculator needed—reason it out.)

- **Drill C (Automation impact):**
  Explain, in 5 bullets, how **CloudFormation + SSM Automation + EventBridge schedules** reduce cost/risk.

**Deliverable:** A half-page “Economics snapshots” sheet (phrases you can drop on the exam).

---

### Block 4 — Integration & Capstone (45–60 min)

- **Teach-Back (Feynman 1-pager):**
  “How AWS creates business value end-to-end”:
  **Value (1.1)** → **Design (1.2)** → **Migration (1.3)** → **Economics (1.4)**.
  One crisp paragraph per step with **service examples**.
- **Capstone Quiz (20 items):**
  10 short-answer explainers + 5 scenario justifications + 5 precise MC traps (performance vs cost; Business vs People; Snowball vs DataSync).

**Deliverables:** 1-pager teach-back + capstone answers.

---

## Assessment Rubric (what “done” looks like)

- **Accuracy:** Pillar/perspective/strategy names and definitions are exact.
- **Application:** You choose correct tools/strategies for scenarios and justify **why**.
- **Service linkage:** Every explanation references **1–2 AWS services** that implement the idea.
- **Clarity:** Plain English, no fluff, short sentences; business value is obvious.

---

## The “Fix-It” Targets We Will Hammer Tomorrow

1. **Performance Efficiency vs Cost Optimization**

   - _Speed vs Spend_ cue, with examples.

2. **CAF Business vs People**

   - _Leadership KPIs vs Training/Roles_ cue.

3. **Migration tool selection**

   - The **Snowball/DataSync/DMS** one-liners + when to pick each.

4. **Compliance framing**

   - Lead with **Region choice**; follow with **Artifact + encryption + CloudTrail/Config**.

5. **Always name services**

   - Build the habit: every answer → 1–2 services.

---

## What to Bring to the Session

- Your **answers** to the WAF matrix, CAF matrix, 6 R’s table, Economics snapshots, and a draft of the **teach-back** page.
- I’ll **grade line-by-line** and then hit you with the **capstone**.

---

If you want, I can also spin those drills into a single downloadable **“Day 2 Packet”** next time so you can fill it in as you go.
