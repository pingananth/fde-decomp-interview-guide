# Sample Interview Questions — Decomposition Round

This collection of real-world problem decomposition questions was sourced from user interviews with FDEs, aspiring FDEs, and hiring managers across tech companies, consulting firms, and AI labs.

Use these scenarios to practice the 5-step decomposition framework detailed in the [README](../README.md#framework) and evaluate your performance against the [7-Signal Rubric](../rubrics/decomposition-round.md).

---

## Question Bank

### Question 1: Healthcare AI Deployment
> *"A large hospital system wants to use AI to reduce medication errors. How do you approach this?"*

- **Key Focus Areas:** Clarifying workflow points (prescribing vs. dispensing vs. administration), HIPAA compliance, legacy EHR system integration (Epic/Cerner), false-positive alarm fatigue, human-in-the-loop validation.

---

### Question 2: Financial Services / LLM Integration
> *"A hedge fund wants to use LLMs to improve their research process. Where do you start?"*

- **Key Focus Areas:** Data privacy/air-gapping, proprietary data leaks, latency requirements, unstructured financial document parsing (10-K filings, earnings transcripts), accuracy vs. hallucination risk.

---

### Question 3: System Adoption & Diagnostics
> *"A logistics company's AI dispatch system has been live for 6 months and adoption is at 30%. What's happening and what do you do?"*

- **Key Focus Areas:** Root-cause analysis (separating technical flaws from UI/UX friction and change management issues), telemetry data collection, driver/dispatcher interviews, phased remediation plan.

---

### Question 4: Rapid Prototyping & Technical Constraints
> *"A 50-person fintech startup wants to reduce customer support tickets by 40% using AI. They have 2,000 old support tickets in CSV format. The CEO wants a demo in 2 weeks. You are the FDE."*

- **Key Focus Areas:** Managing aggressive deadlines, rapid data cleaning and categorization, baseline metrics vs. target expectations, choosing lightweight RAG vs. classification models, scoping a pragmatic 2-week MVP.

---

### Question 5: Supply Chain & Cold Chain Logistics
> *"A national logistics company wants to reduce spoilage in its cold chain. Go."*
*(Reported from a BCG interview loop)*

- **Key Focus Areas:** IoT sensor data ingestion, anomaly detection, predictive route adjustments, operational playbooks for drivers/warehouse staff, ROI and cost-benefit analysis.

---

### Question 6: Enterprise Security & Incident Response
> *"You are at a bank that got a fraud alert. How do you diagnose and resolve it?"*

- **Key Focus Areas:** Immediate containment protocols, root-cause investigation (data drift vs. attack vector), rule update deployment pipelines, regulatory audit trail requirements.

---

## How to Practice with These Questions

1. **Timeboxing:** Set a 30–45 minute timer for each question.
2. **Apply the 5-Step Framework:**
   - **Step 1: Clarify:** Goal, users, technical/business constraints, available data.
   - **Step 2: Decompose:** MECE sub-problems (e.g., Data, Model, Workflow, Adoption).
   - **Step 3: Prioritize:** Identify the highest-leverage bottleneck.
   - **Step 4: Phased Plan:** MVP $\rightarrow$ Enterprise rollout.
   - **Step 5: Name Risks:** Explicit trade-offs and failure modes.
3. **Mocking with LLMs or Peers:** Have a peer or LLM act as the customer stakeholder to test your clarifying questions and narration under pressure.
