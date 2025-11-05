# Full Session Recap — Domain 1 (Cloud Concepts)

## 0) Setup & Scope

- We locked the scope to **Domain 1** from your Lesson Plan:
  **1.1 Benefits**, **1.2 Well-Architected (WAF)**, **1.3 CAF & migration**, **1.4 Cloud economics**.
- Goal for the day: go beyond recognition → **explain concepts in your own words** and **apply** them.

---

## 1) 20-Question Domain 1 Exam (MCQ, multi-select, scenarios)

- You answered all 20 with explanations.
- **Initial score:** 18/20.
  **Correction:** You flagged a typo on Q3 (Economies of Scale); your reasoning matched “B,” updated score **18/20 (90%)**.

### Missed items & fixes

- **Q4 – Data migration (200 TB):**
  You chose **DataSync**; correct is **Snowball**.
  **Why:** DataSync = network-based/ongoing; **Snowball** = bulk **offline** tens–hundreds of TB.
  **Heuristic:**

  - <10 TB → DataSync
  - 10–100s TB → Snowball
  - > 1 PB → Snowmobile

- **Q18 – ESG pillars:**
  You chose **Sustainability + Performance Efficiency**; correct is **Sustainability + Cost Optimization**.
  **Why:** cost optimization directly reduces waste/energy via right-sizing/turning off idle—ESG impact.

### Strengths from this set

- Clear grasp of **WAF pillars**, **capex→opex**, **elasticity vs scalability**, **CAF scope**.
- You consistently tied **technical features to business value**—that’s the exam’s bias.

---

## 2) Deep Dive: WAF (6 pillars) & CAF (perspectives + 6 R’s)

You asked for a deep drill; we covered:

- **WAF:** Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, Sustainability.
  Focus points: automation (IaC), least privilege & traceability, HA/Multi-AZ, right-sizing & serverless, spend visibility & pricing models, environmental impact.
- **CAF:** 6 perspectives (Business, People, Governance, Platform, Security, Operations) and **6 R’s** (Rehost, Replatform, Repurchase, Refactor, Retire, Retain).
  Emphasis: CAF = **organizational strategy & change**; WAF = **workload architecture**.

---

## 3) 30-Question CAF/WAF Gauntlet (harder, trickier)

- You completed all 30. **Score:** **28/30 (93%)**.

### The two misses & why they matter

- **Q6 – Performance Efficiency vs Cost Optimization:**
  You picked “eliminating unused resources” (that’s Cost).
  Performance Efficiency = **matching resource type/size to workload** (right tool for speed/scale), not just reducing waste.
- **Q25 – Business vs People perspective (CAF):**
  CIO/leadership alignment/value realization = **Business** perspective.
  **People** = training, skills, org change mgmt.

**Takeaway:** Watch for **context words**:

- _performance, scaling, architectures_ → Performance Efficiency.
- _waste, spend, idle, pricing_ → Cost Optimization.
- _leadership, KPIs, ROI_ → Business perspective.
- _training, roles, culture_ → People perspective.

---

## 4) Open-Ended “Explain It Back” (Domain 1) — Your Answers + Feedback

### Q1–Q3 (Benefits of AWS Cloud)

- **Economies of Scale:** Nailed it—AWS’s massive scale reduces per-unit costs → savings passed through pay-as-you-go.
- **Global Infra & Latency:** Strong linkage of Regions/AZs/Edge; mention of **data residency** would make it airtight.
- **Agility vs Elasticity vs Scalability:** Excellent. Tiny polish: elasticity = **automatic** response; scalability = **ability** to grow (manual or automatic).

### Q4–Q8 (More Benefits + Compliance)

- **CapEx → OpEx:** Great detail (hardware, power, space, staff). Add the money phrase: **“shifts fixed costs to variable costs.”**
- **HA vs Fault Tolerance:** Excellent distinction—HA tolerates failure with minimal downtime; FT aims for **zero** downtime, **active/active**.
- **Global in Minutes:** Good. Add concrete services: **CloudFront** (CDN), **Route 53** (global DNS), **Elastic Beanstalk/ECS/Lambda** (rapid deploy).
- **Speed of Experimentation:** Correct—pay-as-you-go reduces risk. Add **automation/IaC** as the accelerator.
- **Compliance & Sovereignty:** Good call on **AWS Artifact** and encryption. Add the big lever: **choose the Region** to keep data **in-country**.

---

## 5) Reasoning Quality Audit (from your earlier 20Q)

I scored your **reasoning**, not just answers:

- **10 Excellent**, **6 Strong**, **1 Fair** → avg ~**4.5/5**.
- Where “Strong” became “Excellent”: you named **specific AWS services** implementing the concept (CloudFormation, Budgets, DMS, CodePipeline, etc.).

---

## 6) Your Current Profile (Domain 1)

- **What’s rock-solid:**

  - WAF pillars (names, meanings, examples).
  - CAF 6 R’s (accurate, with scenarios).
  - CapEx→OpEx, elasticity vs scalability, HA vs FT.
  - Mapping tech features → business value.

- **What to polish (specific & actionable):**

  1. **Performance Efficiency vs Cost Optimization** (right-sizing context).
  2. **CAF Business vs People** (leadership outcomes vs training).
  3. **Migration tools** (Snowball vs DataSync vs DMS) with a one-liner decision rule.
  4. **Compliance**: make “**choose the Region**” your first sentence; follow with **Artifact**, **encryption**, **CloudTrail/Config**.
  5. **Always name a service** in explanations (1–2 is enough).

---
