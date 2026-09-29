<div align="center">

# Hwang Junsoo (황준수)

### I build AI systems whose output a person can check.

Backend engineer at 한국리서치. I ship LLM and agent systems into real workflows,
and the part I care about is the part that comes after generation — the gate, the
trace, the audit line that tells you whether the answer can be trusted.

[Portfolio](https://dingmon1019.github.io/) · [Notion](https://www.notion.so/8ae20828d4ce44a695d2c7949b4989b8) · [Email](mailto:jsjsjsjsjs1019@naver.com)

</div>

---

## What I've built

### [tuto](https://github.com/dingmon1019/YoutubeAnalyzer) — evidence-tracked video understanding
`Python` · `MIT` · Claude Code plugin

The values that matter in a tutorial are often never spoken. They sit on screen, and
auto-captions get them wrong — `1536` becomes `136`, and an agent that follows the
caption builds 136-dimensional vectors that fail on every call.

tuto reads the frames. Every knowledge item carries a timestamp, and items grounded in
actual pixels are counted separately from items paraphrased off captions, so you can
see which is which. When captions and screen disagree, the screen wins and the conflict
is kept as structured data rather than smoothed into prose. Merging, cross-checking and
the audit line are deterministic Python; exactly one call goes to the model.

I chose the architecture by measuring it rather than guessing. Six configurations on the
same 54-minute video over one day: **$11.12 → $4.75 (−57%)**, screen-grounded settings
**12 → 40**. Three results ran against my intuition, and measurement won each time.
Benchmark run: 171 knowledge items, 69 screen-grounded, 0% uncited. 785 regression tests.

The limitations are in the README too, including the ones I have not solved.

### [Search-Pro](https://github.com/dingmon1019/Search-Pro-Text-to-SQL) — schema-grounded Text-to-SQL
`C#` · [Python demo](https://github.com/dingmon1019/searchpro-py-demo)

Every data question in the team became a SQL request aimed at a developer. I led the
internal AI contest team as its only engineer, defined the requirements with the people
who actually run the queries, and shipped it.

The design rule was that the model never emits SQL. It returns a structured plan; the
server renders the SQL; a read-only validation gate decides whether it runs. Failures
are sorted into eight types and kept as regression tests. Quote work went from about
40 minutes per case to roughly 4, across ~490 cases a year.

### [star-coach-analysis](https://github.com/dingmon1019/star-coach-analysis) — explainable swing coaching
`Python` · HCI Korea 2026

Pose-correction models hand back a fixed skeleton and no reason. STAR-Coach traces the
optimization that produced the correction and generates the explanation from it: which
body part, at what point in the swing, by how much. This repo is a mock-data
reimplementation of the correction-analysis pipeline from the paper.

### [evaluation-awareness-transfer](https://github.com/dingmon1019/evaluation-awareness-transfer-proposal) — research proposal
`proposal stage — no experiments run yet`

Recent work shows small LLMs internally distinguish "I am being evaluated" from ordinary
use, readable with a linear probe — all of it in English. The proposal asks whether an
English-trained probe survives Korean and Japanese input in 1–4B open models, and
measures an in-language ceiling alongside it so that transfer failure can be told apart
from the representation simply not being there.

Single researcher, ~9 hrs/week, one RTX 3060. The scope is set to fit that.

---

## Publication

**Explainable AI-powered Baseball Swing Coaching System**
Seunghyun Oh, Junsoo Hwang — *Proceedings of HCI Korea 2026*, pp. 1518–1523, Feb. 2026. Equal contribution.

---

## Engineering background

**한국리서치 — Backend Engineer** (2024.09 – present), 온라인패널조사부

ASP.NET Core and Web Forms, SQL Server schema and query work, IIS on Windows Server.
Legacy code, operational risk, unclear requirements, verification cost. That environment
is where the habit came from: before shipping anything a model produced, ask what
evidence would make this output checkable.

`C#` `Python` `Java` `TypeScript` · `ASP.NET Core` `Spring Boot` `React` · `MSSQL` `IIS` `Nginx`

---

## What I'm working on next

Making agent output verifiable is the thread through all of the above, and it is what I
want to keep working on — whether an explanation is faithful or merely plausible, which
parts of an agent trace actually help someone debug a failure, and how to catch SQL and
other generated artifacts that are wrong but entirely convincing.

---

**Contact** · [jsjsjsjsjs1019@naver.com](mailto:jsjsjsjsjs1019@naver.com) · [Portfolio](https://dingmon1019.github.io/) · [Notion Portfolio](https://www.notion.so/8ae20828d4ce44a695d2c7949b4989b8)
