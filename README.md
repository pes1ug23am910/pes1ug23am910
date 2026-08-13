# Hi, I'm Yash Verma 👋

**Final-year B.Tech — Computer Science (AI-ML)** @ PES University, Bengaluru (2023–2027) · **CGPA 8.96/10**, merit scholarship every semester to date

I build reliability-focused systems in Rust, TypeScript, and Python, and applied-ML systems end to end — with real test suites, CI, and honest status reporting. Co-author + **Best Presenter, ICCEE 2026**; first-author NLP study in preparation. Seeking SDE / backend / systems and AI-ML internships and 2027 new-grad roles.

---

## 🔧 Featured Projects

### [micro-raft](https://github.com/pes1ug23am910/micro-raft)
> Raft consensus implemented from scratch in Rust — no consensus libraries of any kind — as a 3-node key-value store over TCP. Leader election, log replication with conflict-only repair, and the Figure-8 current-term commit rule, over durable storage with atomic hard-state swap and torn-tail recovery. The consensus core is I/O-free, so identical code runs against real sockets and against a virtual network.
>
> `Rust` `Cargo workspace` `TCP` — deterministic virtual-time simulator asserting Election Safety / Log Matching / State Machine Safety after **every** step; failures replay from their seed

### [Factuality-First RAG](https://github.com/pes1ug23am910/Factuality-First-RAG)
> Adaptive retrieval-augmented generation: a zero-cost logit/entropy probe decides *when* to retrieve, RoBERTa-large-NLI scores passages, and hybrid FAISS-HNSW + BM25 retrieval runs over a 545k-passage index. 4-bit quantised Mistral-7B inference; claim-level provenance evaluation (FactScore-style).
>
> `Python` `Mistral-7B` `FAISS` `RoBERTa-NLI` `BM25` — pytest + ruff + mypy via GitHub Actions

### [Why VLMs Fail on Indic Memes](https://github.com/pes1ug23am910/Indic_VLM_Taxonomy)
> First-author, pre-registered study (OSF, Apr 2026): an 8-stage evaluation pipeline over a 109-meme Hindi–English code-mixed benchmark. **88.5%** (95% CI 80–95) of GPT-4o and Gemini-2.5-Flash errors trace to missing cultural knowledge — model-invariant. Manuscript in preparation.
>
> `Python` `Multi-VLM harness` `Pre-registration` `Bootstrap CIs`

### [StudyBuddy AI](https://github.com/pes1ug23am910/study-buddy-final)
> Multi-agent tutoring system on Google ADK + Gemini 2.0 Flash: one orchestrator + 5 specialist agents + 3 validator loop-agents routing tutoring, study planning, adaptive quizzing, and progress analytics. 7-stage adaptive spaced repetition (Ebbinghaus curve) with JSON-based cross-session continuity.
>
> `Python` `Google ADK` `Gemini 2.0 Flash` `asyncio`

### [FocusMe](https://github.com/pes1ug23am910/FOCUSME_DUMMY)
> Cross-platform focus-enforcement system in Rust — Windows (WFP) backend implemented and end-to-end tested, remaining backends in progress (status matrix in repo). SQLCipher-encrypted policy store; Axum backend with JWT auth and multi-device policy sync.
>
> `Rust` `Tauri` `React` `TypeScript` `Axum` `PostgreSQL`

## 🧪 Also building (private / local for now)

- **ASCEND** — hybrid event-log/cached-projection desktop productivity RPG (Rust, Tauri 2, React, TypeScript): 11 replayable gameplay/economy projections rebuild from the append-only event log; core economy mutations pair cache and event writes in one SQLite transaction, with compensating transactional undo. **456 automated tests** (327 Rust + 129 Vitest).
- **LocalDocForge** — privacy-first local document processing: typed Python core library, Typer CLI, and a token-authenticated loopback FastAPI service with Job-Object-contained workers. 639-outcome test suite (636 passed, 3 documented platform skips at the last gated merge); hash-locked dependency profiles; reproducible-build gate.
- **PromptGFM-Bio** — prompt-conditioned graph model for rare-disease gene ranking (PyTorch Geometric, frozen PubMedBERT, FiLM conditioning); manuscript in preparation.
- **UI-Migration Capstone (Lead)** — React Native → Kotlin via a typed intermediate representation, with CodeT5+ (220M ×2) encoders; frozen-instrument exact-match reconstruction rose 17.8% → 85.6% across model versions.

## 📄 Research & Publications

- **An Engineering-Oriented ML Decision Support System for Outcome Prediction in Dynamic Environments** — ICCEE 2026 (19th Int'l Conference on Computer & Electrical Engineering, Brisbane) · IOS Press proceedings · Paper IC-1015 · **Co-author, accepted & presented** — and **Best Presenter** award for the presentation.
- **Why VLMs Fail on Indic Memes: A Failure Taxonomy of Cultural-Knowledge Gaps** — first author · pre-registered (OSF, Apr 2026) · manuscript in preparation.

## 🏅 Achievements

- **Best Presenter — ICCEE 2026**, Brisbane (co-sponsored by Central Queensland University), for the online presentation of co-authored paper IC-1015
- **Selected — ISRO research internship**, Space Applications Centre (SAC), Ahmedabad (SRTD, May 2026); could not join due to an academic-calendar conflict
- **Prof. MRD Scholarship** — top 5% of CS (AI-ML), Sem 1 (SGPA 9.36) · **Prof. CNR Scholarship** — top 25%, Sems 2–5
- **Google × Kaggle 5-Day AI Agents Intensive** — multi-agent systems, tool use & orchestration (Google ADK), Nov 2025

## 🛠️ Tech Stack

| | |
|---|---|
| **Languages** | Python, Rust, TypeScript, JavaScript, Kotlin, C, SQL |
| **ML / AI** | PyTorch, PyTorch Geometric, HuggingFace Transformers, BERT / PubMedBERT, FAISS, XGBoost, Google ADK, Scikit-learn |
| **ML Concepts** | RAG, GNNs, NLI, transfer learning, model quantization, vector search, multi-agent orchestration, evaluation design (bootstrap CIs, pre-registration) |
| **Systems & Desktop** | Electron, Tauri 2, Node.js, React, Win32, Axum, Flask, FastAPI, PostgreSQL, REST APIs |
| **Reliability & Testing** | Event sourcing, atomic persistence & crash recovery, IPC security boundaries, Rust / Vitest / Node / pytest testing, GitHub Actions CI/CD |
| **Tools** | Git, Docker, Linux, Weights & Biases, Gemini / OpenAI / Anthropic APIs |

## 📦 Earlier projects

[Japanese Novel Translator](https://github.com/pes1ug23am910/japanese-novel-translator) · [Kakuyomu Translator](https://github.com/pes1ug23am910/kakuyomu-translator) · [Novel Scraper Toolkit](https://github.com/pes1ug23am910/novel-scraper-toolkit) · [Study Tracker](https://github.com/pes1ug23am910/study-tracker) · [Notion-Anki Sync](https://github.com/pes1ug23am910/notion-anki-sync) · [Habitify Dashboard](https://github.com/pes1ug23am910/habitify-dashboard) · [Python Utility Tools](https://github.com/pes1ug23am910/python-utility-tools) · [Cab Aggregator](https://github.com/pes1ug23am910/cab-aggregator-wifly)

## 📊 GitHub Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=pes1ug23am910&show_icons=true&theme=tokyonight)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=pes1ug23am910&layout=compact&theme=tokyonight)

## 📫 Contact

- **Email:** [vermayash16082003@gmail.com](mailto:vermayash16082003@gmail.com)
- **LinkedIn:** [linkedin.com/in/yash-verma-25a1a83a9](https://www.linkedin.com/in/yash-verma-25a1a83a9)
- **University:** PES University, RR Campus, Bengaluru

---

> _"The best code is the code you actually use every day."_
