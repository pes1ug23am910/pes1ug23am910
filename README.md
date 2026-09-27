# Hi, I'm Yash Verma 👋

**Final-year B.Tech — Computer Science (AI-ML)** @ PES University, Bengaluru (2023–2027) · **CGPA 8.96/10** · merit scholarships, Semesters 1–5

I build systems with real test suites and CI, and say plainly what they don't do yet: consensus in Rust, Wi-Fi capture tooling in C, local-first Python services, and evaluation harnesses for ML and LLM systems. Second author of a paper published in the ICCEE 2026 proceedings (Best Presentation award); first-author study on vision-language models in preparation. Seeking SDE / systems / test-engineering and AI-ML internships and 2027 new-grad roles.

---

## 🔧 Featured projects

### [airtrace](https://github.com/pes1ug23am910/airtrace) — 802.11 capture parser and Wi-Fi fault lab
> An allocation-free, bounds-checked C11 parser for pcap/radiotap Wi-Fi captures: 802.11 MAC headers, association/probe/beacon/authentication frames and tagged IEs, status and reason codes, and EAPOL 4-way handshake message classification, with JSONL and statistics output. Verified with 92 unit tests and golden tests checking all 2,273 frames of two public captures against tshark; fuzzed with libFuzzer under ASan/UBSan.
>
> v0.2 adds a Linux `mac80211_hwsim` fault lab (hostapd, wpa_supplicant) that generates labelled connection failures, and an evaluation harness comparing rule-based and LLM triage with frozen test settings and paired statistics. The harness is tested offline; no model results are published yet.
>
> `C11` `radiotap` `libFuzzer` `ASan/UBSan` `Python` `hostapd` `wpa_supplicant`

### [gatehouse-local](https://github.com/pes1ug23am910/gatehouse-local) — credential and quota broker
> A Windows-local API capability broker with typed MCP and CLI interfaces, DPAPI credential custody, revocable sessions and request-bound human approvals. Transactional quota reservations, idempotent usage settlement, and crash recovery that keeps uncertain usage and asynchronous job ownership across restarts.
>
> `Python` `asyncio` `FastAPI` `SQLite WAL` `MCP` `DPAPI` — 3,781 test cases per runtime on Python 3.12–3.14, reproduced by the public Windows CI

### [micro-raft](https://github.com/pes1ug23am910/micro-raft) — replicated key-value store on Raft
> A three-crate Rust system: an I/O-free deterministic Raft core (no consensus library), a fault-injection simulator, and a durable fixed-membership three-node key-value service over Tokio/TCP with an Axum API. Nodes restore term, vote and log on restart and persist before dependent network effects; writes are acknowledged only after application, and unprovable outcomes return `outcome_unknown`.
>
> `Rust` `Tokio` `TCP` `Axum` — 78 tests and a 1,000-seed soak passed (Sep 2026)

### [LocalDocForge](https://github.com/pes1ug23am910/LocalDocForge) — local document processing
> A local document-processing system — typed Python library, CLI, loopback API and MCP server — with 15 engine-gated capabilities, including OCR and Markdown/PDF conversion. Jobs run in fresh resource-bounded workers, and a shared pipeline validates PDF structure and rendering before atomic or collision-safe publication. No uploads, no telemetry.
>
> `Python` `Typer` `MCP` `pikepdf` `PDFium`

### [ASCEND](https://github.com/pes1ug23am910/ASCEND) — local-first productivity RPG
> A Windows desktop app with atomic SQLite transactions coupling task completion, rewards and events, idempotent recurring-period settlement, and single-level compensating undo tested against state reconstructed across 11 domains.
>
> `Rust` `Tauri 2` `React` `TypeScript` `SQLite` — 456 tests passed (327 Rust, 129 frontend; Sep 2026)

### [Why VLMs Fail on Indic Memes](https://github.com/pes1ug23am910/Indic_VLM_Taxonomy) — research, first author
> An evaluation pipeline and error taxonomy for GPT-4o and Gemini-2.5-Flash on 109 Hindi-English memes: 78 of 88 verified errors (88.6%) were cultural-context failures. Pre-registered on OSF (Apr 2026); manuscript in preparation.
>
> `Python` `Jupyter` `evaluation design`

## 📄 Publications and research

- **An Engineering-Oriented Machine Learning Decision Support System for Outcome Prediction in Dynamic Environments** — Detroja, **Verma**, Veena R S, Sushmitha S. *Advances in Transdisciplinary Engineering* 97, pp. 174–184, IOS Press, 2026. [DOI 10.3233/ATDE260666](https://doi.org/10.3233/ATDE260666) · **Best Presentation award**, ICCEE 2026 (Brisbane; presented online).
- **Why VLMs Fail on Indic Memes: A Failure Taxonomy of Cultural-Knowledge Gaps** — first author · pre-registered (OSF, Apr 2026) · manuscript in preparation.
- **PromptGFM-Bio** — phenotype-conditioned gene ranking (BiomedBERT + GraphSAGE + FiLM) over 44,195 genes; a 60-run controlled study with Holm-corrected bootstrap analysis · manuscript in preparation (code private for now).

## 🧪 Other work

- **React Native → Kotlin migration pipeline** (college capstone, designed and built end to end by me) — a typed intermediate representation plus a Kotlin re-encoder; 85.6% exact type match (77/90) on a frozen instrument, up from 17.8% for the first model version.
- [**Factuality-First RAG**](https://github.com/pes1ug23am910/Factuality-First-RAG) — a modular adaptive-RAG research prototype: a retrieval gate deciding *when* to retrieve, dense and lexical retrieval, NLI passage scoring, generation, and evaluation stages. Real-model evaluation is pending.
- [**StudyBuddy**](https://github.com/pes1ug23am910/study-buddy-final) — a console learning-assistant prototype on Google ADK: an orchestrator routing planner, tutor, quiz and progress-tracker agents.
- [**Mini-Raft**](https://github.com/pes1ug23am910/Mini-Raft_Group_12) — a Raft mini-implementation on a Docker Compose cluster (PES University group project).

## 🏅 Achievements

- **Best Presentation award** — ICCEE 2026, Brisbane, for the co-authored paper above
- **Selected** for an ISRO research internship, Space Applications Centre (SAC), Ahmedabad (SRTD, May 2026); couldn't join because of an academic-calendar clash
- **Prof. MRD Scholarship** — top 5% of CSE (AI-ML), Semester 1 (SGPA 9.36) · **Prof. CNR Scholarship** — top 25%, Semesters 2–5
- **Google × Kaggle 5-Day AI Agents Intensive** — Nov 2025

## 🛠️ Tech stack

| | |
|---|---|
| **Languages** | Python, Rust, C, TypeScript, JavaScript, Kotlin, SQL |
| **Systems & testing** | Tokio, Axum, FastAPI, Tauri 2, SQLite, pytest, Vitest, Unity, libFuzzer, ASan/UBSan, GitHub Actions |
| **Networking** | 802.11 / radiotap / EAPOL, pcap, tshark, hostapd, wpa_supplicant, mac80211_hwsim, TCP |
| **ML / AI** | PyTorch, PyTorch Geometric, Hugging Face Transformers, FAISS, scikit-learn, Google ADK, OpenAI-compatible LLM APIs |
| **Practices** | Crash recovery and atomic persistence, deterministic simulation, fault injection, pre-registered evaluation, bootstrap CIs |

## 📦 Earlier projects

[Japanese Novel Translator](https://github.com/pes1ug23am910/japanese-novel-translator) · [Habitify Dashboard](https://github.com/pes1ug23am910/habitify-dashboard) · [Python Utility Tools](https://github.com/pes1ug23am910/python-utility-tools) · [PDF Annotation Extractor](https://github.com/pes1ug23am910/pdf-annotation-extractor) · [Notion Equation Converter](https://github.com/pes1ug23am910/notion-equation-converter) · [Cab Aggregator](https://github.com/pes1ug23am910/cab-aggregator-wifly) (team project)

## 📫 Contact

- **Email:** [vermayash16082003@gmail.com](mailto:vermayash16082003@gmail.com)
- **LinkedIn:** [linkedin.com/in/yash-verma-25a1a83a9](https://www.linkedin.com/in/yash-verma-25a1a83a9)
- **University:** PES University, RR Campus, Bengaluru

---

> _"The best code is the code you actually use every day."_
