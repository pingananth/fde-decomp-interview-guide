# FDE Interview Prep — Decomposition & Client Simulation Rounds

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

## Why This Resource Exists

Plenty of content online explains what a Forward Deployed Engineer (FDE) does. Almost none of it explains how to prepare for the interview — specifically the rounds that trip candidates up most: **problem decomposition** and **client simulation**. 

This repo is scoped narrowly to those two rounds, on purpose. For system design, take-homes, and behavioral prep, see [Resources for Preparation](resources.md) — this guide complements those, it doesn't try to replace them.

---

## Common Mistakes

- **Preparing for LeetCode only:** FDE rounds test structured thinking under ambiguity, not algorithm recall.
- **Solving before clarifying:** Jumping to *"I'd build a dashboard"* in the first two minutes is the single most common failure mode (see Signal 1 in the [Rubric](rubrics/decomposition-round.md)).
- **Treating assumptions as facts:** Building a plan on an unvalidated premise without flagging it.
- **Asserting one "best" answer:** No alternatives named, no trade-offs discussed.
- **Going silent under pressure:** Losing narration exactly when the interviewer adds complexity.

---

## What's Actually Being Tested

Not raw coding ability — **structured thinking, communication under ambiguity, and judgment about real-world constraints** (compliance, legacy systems, team capacity).

The [7-Signal Rubric](rubrics/decomposition-round.md) breaks this down concretely across key engineering behavior dimensions.

---

## HM Rubric — Decomposition Round (7 Signals)

| Signal | Weak | Adequate | Strong |
| :--- | :--- | :--- | :--- |
| **1. Clarify before you solve** | Proposes a solution in the first 2 minutes | Asks 1–2 questions before solving | Establishes goal, constraints, users, data, and success definition before touching a solution |
| **2. MECE decomposition** | Single-dimension or no structure; overlapping sub-problems | Segments along 1–2 dimensions; some gaps remain | Multiple dimensions, mutually exclusive and collectively exhaustive; separates root causes from symptoms |
| **3. Assumption management** | Treats assumptions as facts | States 1–2 assumptions when prompted | Proactively labels assumptions, states what changes if each proves false, revisits as new info arrives |
| **4. Trade-off reasoning** | Asserts one "best" approach, no alternatives | Names two options, picks one with brief reason | Names 2+ approaches, compares on cost/latency/complexity/maintainability, picks one given this customer's specific constraints |
| **5. Edge cases & failure modes** | Designs only for the happy path | Mentions failure modes when asked | Proactively thinks through what breaks each component; fault tolerance is first-class from the start |
| **6. Constraint mapping** | Designs in a vacuum — ignores compliance, legacy systems, data residency | Asks about one or two constraints | Maps technical, operational, and business constraints early; names specifics (air-gap, SSO, FedRAMP) unprompted |
| **7. Narration under pressure** | Goes silent then delivers a conclusion | Narrates when comfortable, drifts into silence when it gets hard | Maintains coherent narration continuously, even as the interviewer adds complexity |

> [!NOTE]
> Weak $\rightarrow$ Adequate $\rightarrow$ Strong is a spectrum, not a checklist. Most candidates land "Adequate" on 4–5 signals and "Weak" on the rest — that's the gap this repo targets.
>
> 📖 **[View the full detailed rubric break-down](rubrics/decomposition-round.md)**

---

## Rounds Covered

- **Decomposition round:** Ambiguous business problem, no clean answer, evaluated on the 7 signals above.
- **Client simulation round:** Roleplay with an interviewer acting as a stakeholder/client; rubric coming soon (contributions welcome).
- **Not covered here:** System design deep-dives, take-homes, pure behavioral — see [Resources for Preparation](resources.md).

---

## Framework

A repeatable process for the decomposition round:

1. **Clarify** — Goal, users, constraints, available data
2. **Decompose** — Break the problem into MECE sub-problems
3. **Prioritize** — Pick the highest-leverage sub-problem first
4. **Propose a phased plan** — Not a final static architecture
5. **Name the risks you're accepting** — Explicitly, not implicitly

> 🎥 See this framework applied in practice $\rightarrow$ [Watch full mock decomposition interview walkthrough](https://www.youtube.com/watch?v=0DeNgIJxa_Y)

---

## Tips

- **Structured thinking & communication:** Structure is what's being graded, not just the answer.
- **Explain why, not just what:** Reasoning is the signal, conclusions are secondary.
- **Check with the interviewer on direction:** This is a working session, not a monologue.
- **Call out trade-offs explicitly:** Don't let the interviewer infer what you considered and rejected.

---

## Sample Interview Questions — Decomposition Round

Sourced from user interviews with FDEs, aspiring FDEs, and hiring managers:

1. *"A large hospital system wants to use AI to reduce medication errors. How do you approach this?"*
2. *"A hedge fund wants to use LLMs to improve their research process. Where do you start?"*
3. *"A logistics company's AI dispatch system has been live for 6 months and adoption is at 30%. What's happening and what do you do?"*
4. *"A 50-person fintech startup wants to reduce customer support tickets by 40% using AI. They have 2,000 old support tickets in CSV format. The CEO wants a demo in 2 weeks. You are the FDE."*
5. *"A national logistics company wants to reduce spoilage in its cold chain. Go."* *(reported from a BCG interview loop)*
6. *"You are at a bank that got a fraud alert. How do you diagnose and resolve it?"*

👉 **[Explore the full question bank with guidance](questions/decomposition-round.md)**

---

## Company-Specific Notes

*Stub — contributions welcome.* 

If you've interviewed at a specific company for an FDE-track role (e.g., Palantir, OpenAI, Anthropic, Scale AI, C3.ai, BCG X), open a Pull Request with anonymized, non-NDA-violating notes on format and focus areas. See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Resources for Preparation

- **[Simul FDE](https://getsimul.com/)** — Self-paced decomposition & client-simulation interview simulator
- **FDE Academy** — Cohort-based prep program
- **Exponent** — General interview prep with some FDE content
- **Community threads on Blind and Reddit** — Search *"forward deployed engineer interview"*
- **LLMs (Claude, GPT, etc.)** can help you rehearse — but verify their answers against real-world constraints rather than memorizing them; interviewers can tell the difference
- **Watch:** [Full mock decomposition interview walkthrough](https://www.youtube.com/watch?v=0DeNgIJxa_Y)

### Adjacent Prep Guides

- System design focus $\rightarrow$ [manjitsin/fde-interview-prep](https://github.com/manjitsin/fde-interview-prep)
- Broader/general FDE prep $\rightarrow$ [pierpaolo28/Awesome-FDE-Roadmap](https://github.com/pierpaolo28/Awesome-FDE-Roadmap)
- Company-specific guides $\rightarrow$ [cma0232/fde-interview-prep](https://github.com/cma0232/fde-interview-prep)

👉 **[View complete resources reference](resources.md)**

---

## Disclaimer

This guide reflects patterns observed as of 2026 and will drift over time:
- **Varies by region:** US and India hiring bars and formats differ.
- **Titles are inconsistent:** "FDE" is applied loosely across the industry; scope varies by company.
- **Roles are still evolving:** Expect this content to age — that's what contributions are for.

*This resource was put together based on internet research and user interviews with FDEs, aspiring FDEs, and hiring managers. It is not official guidance from any employer.*

---

## Contributing & License

Open to community contributions — see [CONTRIBUTING.md](CONTRIBUTING.md). 

Licensed under the [MIT License](LICENSE).

Built by **Ananth**, creator of [Simul FDE](https://getsimul.com/).
