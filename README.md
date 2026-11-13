# Rathesh R

**Software engineering across Android, BLE tooling, and AI systems**

I build things you can install, inspect, and judge: mobile apps with real device constraints, small web companions, and retrieval prototypes that cite their sources.

[Beacon Simulator](https://github.com/ratheshr8/beacon-simulator) · [reasoning-rag `v0.1.0`](https://github.com/ratheshr8/reasoning-rag/releases/tag/v0.1.0) · [Siding `v1.0.0`](https://github.com/ratheshr8/android-auto-stream/releases/tag/v1.0.0) · [ratheshworld.com](https://ratheshworld.com)

## Focus

- **Android / Kotlin / Compose** — BLE advertising and scanning, permissions, and UX that survives OEM quirks
- **Proximity and floor mapping** — QR pairing, multilateration from shared RSSI, webhook integration
- **AI architecture** — hierarchy-aware retrieval, bounded planners, evaluation and threat models you can open
- **Integration honesty** — APIs and platforms documented by what they preserve and what they drop

## Featured projects

### [Beacon Simulator](https://github.com/ratheshr8/beacon-simulator) — Kotlin · Jetpack Compose · MIT

Android app for testing beacon-aware software without physical iBeacon hardware. Dual-mode: advertise and scan on real phones.

- **Transmitter + receiver** — iBeacon manufacturer payloads (`BluetoothLeAdvertiser` / LE scan), optional Eddystone-UID, RSSI and rough distance
- **QR pairing** — lock a receiver to a specific transmitter instead of chasing duplicate advertisements
- **Floor plan locate** — blank or photo plans, place beacons, range rings, user/transmitter multilateration
- **Multi-receiver Wi‑Fi distance sharing** — two or more phones on the same LAN share RSSI distances so a live marker can be trilaterated
- **Webhook forward** — POST scan (and floor-location) JSON to an external URL for backends or automation

**Floorcast** — Next.js companion under `web/` that ingests those webhooks and plots live floor paths ([PR #1](https://github.com/ratheshr8/beacon-simulator/pull/1)).

**APKs:** [github.com/ratheshr8/beacon-simulator/releases](https://github.com/ratheshr8/beacon-simulator/releases)

Needs physical Android devices with BLE. Emulators are not useful; advertising support and Apple company-ID filtering vary by OEM. Details and caveats live in the repo README.

### [reasoning-rag](https://github.com/ratheshr8/reasoning-rag) — Python · prototype `v0.1.0` · Apache-2.0

Hierarchy-aware document QA: navigate a document tree, cite source ranges, surface conflicts, and abstain when the text does not support an answer.

- Tree-first retrieval with a lexical baseline under the same evaluation protocol
- Bounded planner (depth, nodes, model calls) with inspectable traces
- Local demo with upload limits and an explicit notice before any external model call

| Time | Start here |
| --- | --- |
| 2 minutes | [README](https://github.com/ratheshr8/reasoning-rag) |
| 10 minutes | [Evaluation](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/EVALUATION.md) · [Threat model](https://github.com/ratheshr8/reasoning-rag/blob/master/docs/THREAT_MODEL.md) |
| Design review | [ADR index](https://github.com/ratheshr8/reasoning-rag/tree/master/docs/adr) |

## Other projects

| Project | What it is |
| --- | --- |
| [android-auto-stream](https://github.com/ratheshr8/android-auto-stream) (Siding) | Kotlin parked browser for YouTube and streaming sites on phone or Android Automotive OS. Pauses when the app pauses or the car reports driving restrictions. [APK 1.0.0](https://github.com/ratheshr8/android-auto-stream/releases/download/v1.0.0/Siding-1.0.0.apk) |
| [excel-compatible-spreadsheet-app](https://github.com/ratheshr8/excel-compatible-spreadsheet-app) | Private self-hosted spreadsheet workspace (Next.js + Express + Postgres) integrated with ONLYOFFICE Docs. Not Excel parity; licensing gate still open before any production claim |
| [jira-to-jira-migration-tool](https://github.com/ratheshr8/jira-to-jira-migration-tool) | Python CLI that moves a Jira Cloud project with Postgres checkpoints. README documents which fields the public API cannot preserve |
| [MordenizeCodeConvert](https://github.com/ratheshr8/MordenizeCodeConvert) | React + TypeScript UI for code conversion through Azure OpenAI. Keys stay in local `.env` |
| [Angular-Web-Component-Sample](https://github.com/ratheshr8/Angular-Web-Component-Sample) | Angular Elements data grid packaged as one JS bundle for plain HTML and server-rendered pages |
| [APIGateWay-Ocelot-With-JWT](https://github.com/ratheshr8/APIGateWay-Ocelot-With-JWT) | Local .NET sample: Ocelot gateway, JWT auth server, and a customers API |

## Reference sample

[SMART on FHIR tutorial](https://github.com/ratheshr8/-smart-on-fhir-tutorial) is a labeled learning copy of the public SMART on FHIR example (EHR sandbox → `Patient` / selected `Observation`s). Sandbox tutorial only — not a clinical product.

## How I work

Lead with artifacts a reviewer can clone, install, or open: release APKs, ADRs, evaluation notes, and explicit limitations. Prefer stating platform and API boundaries over marketing claims.
