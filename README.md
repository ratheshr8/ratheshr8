# Rathesh R

**AI Architecture & Engineering | Agentic Systems | AI Governance**

I design systems that can show their work: retrieval with citations, bounded agent plans, and integration tools with stated limits.

[reasoning-rag `v0.1.0`](https://github.com/ratheshr8/reasoning-rag/releases/tag/v0.1.0) · [Siding `v1.0.0`](https://github.com/ratheshr8/android-auto-stream/releases/tag/v1.0.0) · [ratheshworld.com](https://ratheshworld.com)

## Start here

The flagship is [reasoning-rag](https://github.com/ratheshr8/reasoning-rag), a prototype for hierarchy-aware document QA.

| If you have… | Open |
| --- | --- |
| 2 minutes | [README](https://github.com/ratheshr8/reasoning-rag) — problem, what works, quickstart |
| 10 minutes | [Evaluation protocol](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/EVALUATION.md) and [threat model](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/THREAT_MODEL.md) |
| A design review | [ADR index](https://github.com/ratheshr8/reasoning-rag/tree/master/docs/adr) — scope, retrieval, planning, eval, demo, release |

## Featured work

### [reasoning-rag](https://github.com/ratheshr8/reasoning-rag) — prototype `v0.1.0` · Python · Apache-2.0

Long technical documents hide answers across sections. This prototype navigates a document tree, cites source ranges, surfaces conflicts, and abstains when the document does not support an answer.

| Decision | Where it shows up |
| --- | --- |
| Tree-first retrieval, with a lexical baseline under the same protocol | [ADR 0005](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/adr/0005-retrieval-baselines.md), [eval-v0](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/EVALUATION.md) |
| Bounded planner (depth, nodes, model calls) and inspectable traces | [ADR 0006](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/adr/0006-query-planning.md) |
| Claims only when citations resolve; conflicts stay visible | [ADR 0007](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/adr/0007-navigation-and-verification.md) |
| Local demo with upload limits and a provider notice before any external model call | [ADR 0009](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/adr/0009-demo-and-api.md) |
| Markdown, synthetic CC0 corpus, local prototype | [Limitations](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/LIMITATIONS.md) |

A vector baseline stays a placeholder until it runs under the same eval rules.

## Also published

These are real public repos with a usable README. They are samples or tools, not the same evidence bar as the flagship.

| Repo | What it is | Look at |
| --- | --- | --- |
| [android-auto-stream](https://github.com/ratheshr8/android-auto-stream) | Siding, a Kotlin parked browser (Apache-2.0) for YouTube and streaming sites on a phone or Android Automotive OS. Playback pauses when the app pauses or the car reports driving restrictions. It does not relabel itself as a game or a navigation app | [Download 1.0.0](https://github.com/ratheshr8/android-auto-stream/releases/download/v1.0.0/Siding-1.0.0.apk). The README states which sites usually play in a WebView and which refuse it |
| [jira-to-jira-migration-tool](https://github.com/ratheshr8/jira-to-jira-migration-tool) | Python CLI (Apache-2.0) that moves a Jira Cloud project — issues, comments, attachments, and best-effort filters/dashboards — with Postgres checkpoints so a run can resume | README section on what the public Jira API cannot preserve (authors, timestamps, full history, admin schemes) |
| [MordenizeCodeConvert](https://github.com/ratheshr8/MordenizeCodeConvert) | React + TypeScript UI (Apache-2.0) for code conversion through Azure OpenAI. Keys stay in a local `.env` | `npm install` / `npm run dev` in the README. This is an app shell, not a measured migration benchmark |
| [Angular-Web-Component-Sample](https://github.com/ratheshr8/Angular-Web-Component-Sample) | Angular Elements data grid (sort, page, row selection) packaged as one JS bundle for plain HTML and Java server-rendered pages | Build (`npm run build:wc`) and the HTML embed snippet in the README |
| [APIGateWay-Ocelot-With-JWT](https://github.com/ratheshr8/APIGateWay-Ocelot-With-JWT) | Local .NET sample: Ocelot gateway, JWT auth server, and a customers API. Demo user and signing secret are set in local appsettings, not committed | [README](https://github.com/ratheshr8/APIGateWay-Ocelot-With-JWT/blob/main/README.md) project table and the route file `APIGateway/configuration.json` |

## Reference sample

[SMART on FHIR tutorial](https://github.com/ratheshr8/-smart-on-fhir-tutorial) is a **reference-only** learning copy of the public SMART on FHIR example. The app launches from an EHR sandbox and reads `Patient` plus a few `Observation` resources (height, blood pressure, cholesterol). Open `index.html` and `example-smart-app/`. The repo README is only a title.

This does not change the headline. It is a sandbox tutorial, not a clinical product and not regulated healthcare delivery.

## Skills you can verify

- **System design** — ADRs that record options and the choice. Start at [ADR 0001](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/adr/0001-project-scope.md).
- **Retrieval and evaluation** — tree-first vs lexical on one versioned dataset. [EVALUATION.md](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/EVALUATION.md).
- **Agent bounds** — query analysis, budgets, and stop conditions in the trace. [ADR 0006](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/adr/0006-query-planning.md).
- **Integration limits** — the Jira migrator documents which fields the Cloud API can and cannot recreate.
- **Platform limits** — what a system WebView will play, and which parked categories Android Auto and Android Automotive accept. [Siding](https://github.com/ratheshr8/android-auto-stream).
- **Governance** — abstention, citation checks, threat model, security reporting. [THREAT_MODEL.md](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/THREAT_MODEL.md).

## How I work

The profile leads with work a reviewer can open and judge. `reasoning-rag` is the architecture proof. The other linked repos are published tools, UI samples, a parked Android browser, or a labeled reference tutorial.
