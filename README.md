### Hi, I'm Arun Rajendiran — AI Product Manager

I spec products, but I also build them: agent orchestration, guardrails, data models, and the UI, end to end, so I can validate product decisions against working software instead of a deck. The three projects below are shipped, live, and each pressure-test a different product skill.

| Project | What it is | What it proves |
|---|---|---|
| **[CreditScout](https://github.com/arunr-mib/creditscout)** — [live](https://credit-scout.vercel.app) | A decision-support agent for commercial credit analysts investigating covenant exceptions | Agentic reasoning with hard guardrails — the model never produces a number; every figure traces to a logged calculation or a verbatim citation, or the system abstains. [Case study →](https://github.com/arunr-mib/creditscout/blob/main/docs/case-study.md) |
| **[SpreadSense](https://github.com/arunr-mib/spreadsense)** — [live](https://spreadsense.vercel.app) | AI-powered financial spreading: PDF financials → extracted to a structured grid, reviewer-confirmed | Full-stack ownership with real CI — FastAPI/Postgres backend, React frontend, GitHub Actions running 75+ backend tests on every push. [Case study →](https://github.com/arunr-mib/spreadsense/blob/main/docs/case-study.md) |
| **[CreditResolve](https://github.com/arunr-mib/CreditResolve)** — [live](https://creditapp-chi.vercel.app/) | A problem-loan workout dashboard prototype | Fast concept exploration — a vibe-coded prototype built to pressure-test a UI concept and domain taxonomy in days, not weeks. [Case study →](https://github.com/arunr-mib/CreditResolve/blob/main/docs/case-study.md) |

Covenant monitoring and financial spreading are both known time sinks for credit analysts — hours spent re-deriving numbers that should already be known. CreditScout and SpreadSense attack that from opposite ends: one investigates the exception, the other compresses the transcription that precedes it.

Each repo's README covers the "what." The case study linked above covers the "why" — the product decisions behind the build, not just the feature list.

One more thing worth reading: **[what I didn't build, and why](./docs/decisions-i-didnt-build.md)** — two real examples of scoping a build down or pausing it, and the reasoning behind each call.

### Credentials

Agentic AI Product Management Certification + Claude Code Official Dev Cert. — Maven, Cohort 10, taught by Mahesh Yadav (Agentic AI Institute). CreditScout was the cohort capstone and won **Best Regulated Tech / Compliance AI** at the cohort's pitch day, recognized for "an orchestrator that investigates loan covenant breaches with cited tools and a learning loop, built for the audit and security expectations of banking."