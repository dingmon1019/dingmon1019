<div align="center">

# Hwang Junsu (황준수)
### Backend Engineer -> XAI / Agent Explainability Researcher-in-Progress

**Turning practical AI engineering experience into testable research questions.**

I am not presenting myself as a finished researcher. I am using backend engineering experience to shape small, testable research questions around XAI, human-verifiable AI outputs, Text-to-SQL evaluation, uncertainty, and agent explainability.

[Research Direction](./research-direction.md) · [Notion Portfolio](https://www.notion.so/8ae20828d4ce44a695d2c7949b4989b8) · [Email](mailto:jsjsjsjsjs1019@naver.com)

</div>

---

## Research Direction

I work as a backend developer in Korea and am preparing for ICML 2026 as a networking and research-direction milestone, not as a paper author.

My current transition is:

> Backend Engineer -> XAI / Agent Explainability Researcher-in-Progress

I am interested in research questions that connect practical engineering constraints with explainability evaluation:

- **Human-Centered XAI**: turning model outputs into feedback that users can understand and act on.
- **Explanation Faithfulness**: evaluating whether heatmaps or explanation maps are faithful to the model's decision process, not only visually plausible.
- **Uncertainty & Calibration**: combining uncertainty signals with explanations so users can judge when an explanation should not be trusted.
- **Agent Explainability**: identifying which parts of an LLM agent trace are actually useful for debugging, accountability, and calibrated trust.
- **Text-to-SQL Evaluation**: helping users verify, debug, and trust generated SQL in schema-grounded enterprise databases.
- **AI-assisted Software Engineering**: evaluating AI coding-agent output through maintainability, testability, and failure analysis, not only pass/fail results.

---

## Publication / Conference Proceeding

**Explainable AI-powered Baseball Swing Coaching System**  
Seunghyun Oh, Junsoo Hwang  
Proceedings of HCI Korea 2026, pp. 1518–1523, Feb. 2026.  
Equal contribution.

This work proposes **STAR-Coach**, an explainable AI-powered baseball swing coaching system. STAR-Coach turns black-box pose refinement into actionable feedback: which body part should be corrected, when correction is needed, how much adjustment is required, and how feedback can be presented visually, quantitatively, and textually.

---

## Engineering Background

My engineering background is in enterprise web systems, database-heavy services, and deployment workflows. I try to keep the research transition grounded in systems that have real constraints: legacy code, operational risk, unclear requirements, and verification cost.

- **Backend**: ASP.NET Core, ASP.NET Web Forms, Spring Boot, Java, C#
- **Database**: MSSQL schema design, stored procedures, views, query optimization
- **Infrastructure**: IIS, Windows virtual servers, Nginx reverse proxy
- **Frontend**: React, Vite, JavaScript/TypeScript
- **AI-assisted workflow**: agentic planning, code review, refactoring support, test generation, QA checklists, failure analysis

The part I want to carry into research is not the claim that AI makes development faster. It is the habit of asking: **what evidence would make this output trustworthy?**

---

## Current Research Questions

```text
1. Explanation Faithfulness
   When an explanation looks reasonable, how do we know whether it reflects the model's actual decision process?

2. Human-Actionable XAI
   How can AI feedback explain not only what is wrong, but what action the user should take next?

3. Agent Trace Evaluation
   Which intermediate steps of an AI agent are useful for debugging, accountability, and calibrated trust?

4. Text-to-SQL Verification
   What trace, schema grounding, or validation signal helps users detect wrong but plausible generated SQL?

5. AI-assisted Software Engineering
   Can real engineering tasks become small benchmarks for evaluating AI coding agents beyond pass/fail tests?
```

---

## Selected Work

These repositories are being reorganized as evidence for the research direction above:

- [Search-Pro: Schema-Grounded Text-to-SQL Assistant](https://github.com/dingmon1019/Search-Pro-Text-to-SQL): sanitized public snapshot of a Text-to-SQL assistant. It translates natural-language questions into a schema-grounded semantic plan, renders read-only SQL server-side, validates query shape, executes against a mock database pipeline, and records traces for human verification. Relevant to Text-to-SQL explainability, query validation, and wrong-but-plausible output detection.
- [HRClaw](https://github.com/dingmon1019/HRClaw): Windows-first local multi-agent runtime with approval, audit, provider routing, bounded connectors, and worker execution records. Relevant to agent trace, accountability, and operator-facing explanations.
- [orchestrator](https://github.com/dingmon1019/orchestrator): plan-driven media production harness with explicit artifacts, schemas, validation gates, and quality bars. Relevant to reproducible agent workflows and artifact-level evaluation.
- [ARIS-research-tool-](https://github.com/dingmon1019/ARIS-research-tool-): forked research-workflow reference for autonomous research loops. Useful as a study/reference repo; it should be pinned only if I add my own adaptation notes or experiments.

More context is tracked in [research-direction.md](./research-direction.md).

---

## Connect

- **Email**: [jsjsjsjsjs1019@naver.com](mailto:jsjsjsjsjs1019@naver.com)
- **Portfolio**: [Notion Portfolio](https://www.notion.so/8ae20828d4ce44a695d2c7949b4989b8)
- **GitHub**: [github.com/dingmon1019](https://github.com/dingmon1019)
