# openkoutsi

A **self-hosted cycling coaching platform**. Upload FIT files or sync from Strava/Wahoo,
track fitness metrics (fitness/fatigue/form), build periodized training plans, and get optional AI
coaching feedback — all on a server you control.

> **koutsi** (κουτσί) — Finnish for "coach"

## 🚴 Try it out

### ➡️ **[koutsi.dev](https://koutsi.dev)** ⬅️

The platform is live at **<https://koutsi.dev>** — that's the landing page; the web app itself
runs at **<https://app.koutsi.dev>**.

## Why

Most cycling coaching tools are cloud-only SaaS. openkoutsi is different: you run it on your
own hardware, your data stays under your control, and integrations are optional. One
deployment is a single instance that many users can share, with every user's athlete profile
and training data kept in their own isolated database.

## Documentation

| Docs | Link |
|---|---|
| 📖 **User guide** — how to use every feature | <https://openkoutsi.github.io/openkoutsi-docs/> |
| 🏛️ **Architecture reference** — how the system fits together | <https://openkoutsi.github.io/openkoutsi-arch/> |

## Repositories

openkoutsi is split across a few repositories:

| Repository | What it contains |
|---|---|
| [**openkoutsi**](https://github.com/openkoutsi/openkoutsi) (this repo) | Project planning and the user-facing issue tracker — report bugs and request features here. |
| [**openkoutsi-backend**](https://github.com/openkoutsi/openkoutsi-backend) | The backend: FastAPI API, the Strava/Wahoo webhook **bridge services**, and the pure-Python `openkoutsi` **core library** (FIT parsing, training math, plan building). |
| [**openkoutsi-web**](https://github.com/openkoutsi/openkoutsi-web) | The web frontend — a Next.js 15 (App Router) app in TypeScript with Tailwind CSS and Recharts. |
| [**openkoutsi-landing-page**](https://github.com/openkoutsi/openkoutsi-landing-page) | The landing page - plain HTML. |
| [**openkoutsi-ops**](https://github.com/openkoutsi/openkoutsi-ops) | Infrastructure-as-code and deployment configuration — a containerized, poll-based deployment that is fully rebuildable from code. |
| [**openkoutsi-docs**](https://github.com/openkoutsi/openkoutsi-docs) | Source for the **user guide** (MkDocs + Material), published to GitHub Pages. |
| [**openkoutsi-arch**](https://github.com/openkoutsi/openkoutsi-arch) | Source for the **architecture reference** (MkDocs + Material), published to GitHub Pages. |
| [**.github**](https://github.com/openkoutsi/.github) | Organisation profile and shared community-health files. |

## Feature requests & bug reports

Found a bug or have an idea? Please open an issue in **this repository**:

- 🐛 **Report a bug:** [open a bug report](https://github.com/openkoutsi/openkoutsi/issues/new?template=bug_report.md)
  using the template — describe what you did, what you expected, and what actually happened.
  Include steps to reproduce and any relevant logs or screenshots.
- 💡 **Request a feature:** <https://github.com/openkoutsi/openkoutsi/issues/new> — describe
  the use case and what you'd like to see.

Before opening a new issue, please [search the existing
issues](https://github.com/openkoutsi/openkoutsi/issues) to avoid duplicates. Issues that
concern a specific component (e.g. a UI glitch or an API bug) may be moved to the relevant
repository, but this tracker is the right place to start.

## License

openkoutsi is licensed under Apache-2.0.
