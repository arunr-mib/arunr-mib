### Hi, I'm Arun Rajendiran, AI Product Manager

I spec products, but I also build them: agent orchestration, guardrails, data models, and the UI, end to end, so I can validate product decisions against working software instead of a deck. The four projects below are shipped, live, and each pressure-test a different product skill.

| Project | What it is | What it proves |
|---|---|---|
| **[CreditScout](https://github.com/arunr-mib/creditscout)** ([live](https://credit-scout.vercel.app)) | A decision-support agent for commercial credit analysts investigating covenant exceptions | Agentic reasoning with hard guardrails: the model never produces a number; every figure traces to a logged calculation or a verbatim citation, or the system abstains. [Case study →](https://github.com/arunr-mib/creditscout/blob/main/docs/case-study.md) |
| **[SpreadSense](https://github.com/arunr-mib/spreadsense)** ([live](https://spreadsense.vercel.app)) | AI-powered financial spreading: PDF financials → extracted to a structured grid, reviewer-confirmed | Full-stack ownership with real CI: FastAPI/Postgres backend, React frontend, GitHub Actions running 75+ backend tests on every push. [Case study →](https://github.com/arunr-mib/spreadsense/blob/main/docs/case-study.md) |
| **[CreditResolve](https://github.com/arunr-mib/CreditResolve)** ([live](https://creditapp-chi.vercel.app/)) | A problem-loan workout dashboard prototype | Fast concept exploration: a vibe-coded prototype built to pressure-test a UI concept and domain taxonomy in days, not weeks. [Case study →](https://github.com/arunr-mib/CreditResolve/blob/main/docs/case-study.md) |
| **[creditapp-evals](https://github.com/arunr-mib/creditapp-evals)** ([scorecard](https://creditapp-evals.vercel.app)) | A multi-product eval harness: signed golden cases, a deterministic grader, a named failure taxonomy | Proof over demos: a deterministic grader (no LLM-as-judge) that fails the build on a hallucinated number or a false resolve. It grades real recorded CreditScout runs (Nov 2026: 3 of 5 cold, 4 of 5 warm, zero false resolves, published with the failures) alongside a hand-written regression suite. Built as a hub: SpreadSense's suite is next. [Case study →](https://github.com/arunr-mib/creditapp-evals/blob/main/docs/case-study.md) |

Covenant monitoring and financial spreading are both known time sinks for credit analysts: hours spent re-deriving numbers that should already be known. CreditScout and SpreadSense attack that from opposite ends: one investigates the exception, the other compresses the transcription that precedes it.

Each repo's README covers the "what." The case study linked above covers the "why": the product decisions behind the build, not just the feature list.

One more thing worth reading: **[what I didn't build, and why](./docs/decisions-i-didnt-build.md)**, two real examples of scoping a build down or pausing it, and the reasoning behind each call.

### Credentials

<a href="https://www.credly.com/badges/eebf2592-4b39-433e-af9c-c1e181417364"><img src="docs/credentials/claude-certified-developer-foundations.png" alt="Claude Certified Developer, Foundations badge, issued by Anthropic" width="110"></a>

- **[Claude Certified Developer, Foundations](https://www.credly.com/badges/eebf2592-4b39-433e-af9c-c1e181417364)** (Anthropic, Nov 2026)
- **Agentic AI Product Management Certification** (Agentic AI Institute, Cohort 10, run on Maven, Oct 2026), taught by Mahesh Yadav, Programme Director. CreditScout was the cohort capstone and won **[Best Regulated Tech / Compliance AI](docs/credentials/agentic-ai-institute-best-regulated-tech.webp)** at the cohort's pitch day. The certificate's citation: "Recognised for an orchestrator that investigates loan covenant breaches with cited tools and a learning loop, built for the audit and security expectations of banking."
