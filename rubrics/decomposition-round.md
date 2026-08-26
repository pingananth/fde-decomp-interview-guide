# HM Rubric — Decomposition Round (7 Signals)

This rubric outlines the 7 key evaluation signals used by hiring managers and interviewers during the Forward Deployed Engineer (FDE) **Problem Decomposition Round**.

Weak $\rightarrow$ Adequate $\rightarrow$ Strong is a spectrum, not a checklist. Most candidates land "Adequate" on 4–5 signals and "Weak" on the rest — that is the gap this guide targets.

---

## The 7-Signal Rubric Table

| Signal | Weak | Adequate | Strong |
| :--- | :--- | :--- | :--- |
| **1. Clarify before you solve** | Proposes a solution in the first 2 minutes | Asks 1–2 questions before solving | Establishes goal, constraints, users, data, and success definition before touching a solution |
| **2. MECE decomposition** | Single-dimension or no structure; overlapping sub-problems | Segments along 1–2 dimensions; some gaps remain | Multiple dimensions, mutually exclusive and collectively exhaustive; separates root causes from symptoms |
| **3. Assumption management** | Treats assumptions as facts | States 1–2 assumptions when prompted | Proactively labels assumptions, states what changes if each proves false, revisits as new info arrives |
| **4. Trade-off reasoning** | Asserts one "best" approach, no alternatives | Names two options, picks one with brief reason | Names 2+ approaches, compares on cost/latency/complexity/maintainability, picks one given this customer's specific constraints |
| **5. Edge cases & failure modes** | Designs only for the happy path | Mentions failure modes when asked | Proactively thinks through what breaks each component; fault tolerance is first-class from the start |
| **6. Constraint mapping** | Designs in a vacuum — ignores compliance, legacy systems, data residency | Asks about one or two constraints | Maps technical, operational, and business constraints early; names specifics (air-gap, SSO, FedRAMP) unprompted |
| **7. Narration under pressure** | Goes silent then delivers a conclusion | Narrates when comfortable, drifts into silence when it gets hard | Maintains coherent narration continuously, even as the interviewer adds complexity |

---

## Detailed Signal Breakdown

### 1. Clarify Before You Solve
- **Why it matters:** FDEs work in highly ambiguous customer environments. Jumping directly into solution mode without understanding business constraints leads to building the wrong thing.
- **How to move to Strong:** Before proposing any architectural component, explicitly ask about:
  - Business objective & success metric (e.g., SLA, accuracy, latency, cost target).
  - Target end-users (technical level, workflow integration points).
  - Existing infrastructure, legacy data formats, and technical constraints.

### 2. MECE Decomposition
- **Why it matters:** Mutually Exclusive, Collectively Exhaustive (MECE) framing ensures complete problem coverage without redundant work.
- **How to move to Strong:** Break down problems along logical axes (e.g., Ingestion $\rightarrow$ Processing $\rightarrow$ Inference $\rightarrow$ Action, or Technical vs. Operational vs. Human Adoption).

### 3. Assumption Management
- **Why it matters:** In real engagements, data availability or technical capability often deviates from initial expectations.
- **How to move to Strong:** Proactively state: *"I am assuming X (e.g., data is structured JSON). If this assumption fails and data is unformatted PDFs, our pipeline shifts to..."*

### 4. Trade-Off Reasoning
- **Why it matters:** There is no single perfect architecture in client engineering; every decision involves compromise.
- **How to move to Strong:** Explicitly frame decisions as trade-offs across cost, complexity, latency, maintainability, and implementation timeline.

### 5. Edge Cases & Failure Modes
- **Why it matters:** Production systems must handle degraded networks, corrupted data, rate limits, and model hallucinations gracefully.
- **How to move to Strong:** Introduce retry loops, fallback mechanisms, dead-letter queues, and human-in-the-loop validation early in the design.

### 6. Constraint Mapping
- **Why it matters:** Enterprise environments enforce strict security, compliance, and governance boundaries.
- **How to move to Strong:** Unprompted, consider compliance frameworks (FedRAMP, HIPAA, SOC2), network isolation (air-gapped deployments, VPC peering), and authentication standards (SAMIL/SSO, RBAC).

### 7. Narration Under Pressure
- **Why it matters:** FDEs interact with technical and non-technical stakeholders under stressful project timelines.
- **How to move to Strong:** Think out loud, structure your verbal delivery ("First, I will look at data ingestion; second, model selection..."), and check in regularly with your interviewer ("Does this direction align with your expectations?").
