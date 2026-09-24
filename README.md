# Hi, I'm Parth Kansal 👋

**AI/ML Engineer** · Full-Stack Builder · B.E. 2027 · India

I build AI-first systems end to end — from data collection and model training to the backend, the dashboard, and the tests that prove it works. Lately that means **ML inside real systems**: a learned query optimizer that steers PostgreSQL, a deception layer that catches web attackers, and a crisis-response network that triages alerts in 8 Indian languages.

I care about measured results: baselines, ablations, confidence intervals, CI on every push, and writing down what *didn't* work.

[![Email](https://img.shields.io/badge/Email-parth.kansal823%40gmail.com-D14836?logo=gmail&logoColor=white)](mailto:parth.kansal823@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-kpartha238-0A66C2?logo=linkedin&logoColor=white)](https://linkedin.com/in/kpartha238)
[![Portfolio](https://img.shields.io/badge/Portfolio-parthkansal823.github.io-111111?logo=githubpages&logoColor=white)](https://parthkansal823.github.io/)
[![Resume](https://img.shields.io/badge/Resume-View-4285F4?logo=googledocs&logoColor=white)](https://docs.google.com/document/d/1CNtW00Nn2qMzzU1lpASgOgzwUMuiFd_F/edit?usp=sharing&ouid=102537288796624398044&rtpof=true&sd=true)

📬 Open to **AI/ML + SWE roles (2026–27)**

---

## 🚀 Featured Work

### 🛡️ [Active Deception Framework for Web Attack Detection](https://github.com/parthkansal823/FinalYearProject-Deception)
*Final-year research project.* A reverse proxy that, when unsure about a visitor, plants invisible bait in responses — a fake SQL error, an unused JSON field, a hint at a deprecated endpoint. Real users never see it; attackers who act on it identify themselves and are silently moved into a state-consistent decoy copy of the site where everything they do is recorded.
- Attack recall **0.889 → 0.943** over the passive baseline across 99 paired seeds (McNemar p ≈ 10⁻⁹⁵), with **0 of 7,920** benign sessions diverted
- Decoy environment with **0.00% contradictions** over 286 consistency probes; tested against scripted, browser-driven and LLM-agent attackers
- Append-only hash-chained logging, per-component fail-open, frozen model manifest, **371 tests**

`Python` `FastAPI` `scikit-learn` `PostgreSQL` `LLM agents` `Security`

### 🧠 [Learned Query Optimizer](https://github.com/parthkansal823/DB_QueryOptimizer)
A learned plan-picking layer on top of PostgreSQL 18, in the spirit of Bao (SIGMOD '21). It generates ~20 alternative plans per query with `pg_hint_plan`, predicts latency and uncertainty with a bootstrapped LightGBM ensemble, and only deviates from PostgreSQL's own plan when it is confident the worst case is bounded.
- Safety veto + per-query regression guard + conformally calibrated confidence gate; self-retraining champion/challenger loop with rollback
- Points at **any PostgreSQL database**: discovers the schema, infers join keys, generates a workload from real data distributions, and trains — evaluated on the JOB/IMDB benchmark (21 tables, 74M rows)
- React dashboard that explains every decision; **1,414 tests** in CI (including live-PostgreSQL integration tests)

`Python` `FastAPI` `LightGBM` `PostgreSQL` `React` `Docker`

### 🆘 [NeighbourAid — Hyperlocal Crisis & Help Network](https://github.com/parthkansal823/NeighbourAid)
Real-time community crisis response for India. People report emergencies with text, GPS, photos or voice; alerts are triaged locally and pushed over WebSockets to skill-matched volunteers nearby.
- In-process multilingual triage across **8 Indian languages** — **90%** accuracy on a labelled set, **17/17** on critical alerts, no API key or per-alert cost
- Composite verification score from community witnesses, corroborating reports, live weather and photo evidence
- 11-language UI, installable PWA with an offline alert queue, live map, volunteer trust scores and live tracking

`Python` `FastAPI` `WebSockets` `React` `MongoDB` `PWA`

---

## 🧩 More Projects

| Project | What it is | Stack |
|---|---|---|
| **[Adaptive_IAM](https://github.com/parthkansal823/Adaptive_IAM)** | AI-powered identity and access management exploring LLM-based authorization and blockchain-assisted trust | `Python` `LLM` `Blockchain` |
| **[Diabetes Prediction using Soft Computing](https://github.com/parthkansal823/Diabetes-Prediction-using-Soft-Computing)** | Disease prediction from structured medical data using fuzzy logic and neural networks | `Python` `Jupyter` `ML` |
| **[CodeChatter](https://github.com/parthkansal823/CodeChatter)** | Real-time developer chat with snippet sharing and collaborative coding | `JavaScript` `Node.js` `WebSockets` |
| **[shopper](https://github.com/parthkansal823/shopper)** | Cal.com-style scheduling and booking with dynamic availability and event configuration | `JavaScript` |
| **[System Log Analyzer & Anomaly Detector](https://github.com/parthkansal823/System-Log-Analyzer-Anomaly-Detector)** | Parses system logs, flags anomalies, and surfaces operational insights | `C++` |

---

## ⚙️ Tech Stack

| Domain | Stack |
|---|---|
| **Languages** | Python · JavaScript · C/C++ · SQL · Java |
| **AI / ML** | PyTorch · scikit-learn · LightGBM · NumPy · Pandas · Jupyter · LLM APIs |
| **Backend** | FastAPI · Node.js · Express · REST · WebSockets |
| **Frontend** | React · Vite · Tailwind CSS · Recharts · Leaflet |
| **Data** | PostgreSQL · MongoDB |
| **Tooling** | Git · GitHub Actions · Docker · Linux · pytest · Vitest |

---

## 🔬 Current Focus

- **ML for systems** — learned query optimization, uncertainty estimation, and knowing when a model should *not* act
- **AI security** — active deception, attack detection, and evaluating defences against LLM-driven attackers
- **LLM systems** — transformers, attention, agents, and practical fine-tuning
- **Engineering fundamentals** — DSA, system design, testing, and shipping end-to-end products

---

I'm looking for high-growth teams building AI-native products and intelligent systems — software that creates measurable value. Say hi at [parth.kansal823@gmail.com](mailto:parth.kansal823@gmail.com).
