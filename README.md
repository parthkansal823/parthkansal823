# Hi, I'm Parth Kansal 👋

**AI/ML Engineer** · Full-Stack Builder · India  
🎓 B.E. Computer Science (Information Security, IBM) · Chandigarh University · 2027

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
*Final-year team project at Chandigarh University · research paper in progress.* A reverse proxy that, when unsure about a visitor, plants invisible bait in responses — a fake SQL error, an unused JSON field, a hint at a deprecated endpoint. Real users never see it; attackers who act on it identify themselves and are silently moved into a state-consistent decoy copy of the site where everything they do is recorded.
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

## 🌐 Full-Stack Products

### 💻 [CodeChatter](https://github.com/parthkansal823/CodeChatter)
Collaborative coding workspace: shared rooms with live presence and cursors, a Monaco editor with file tree and in-room terminal, runnable starter projects (DSA practice in 15 languages), WebRTC video calls and screen sharing, two-way GitHub sync, and optional Gemini-powered AI help. JWT auth with email OTP plus Google/GitHub OAuth.

`React` `FastAPI` `WebSockets` `WebRTC` `MongoDB` `Gemini`

### 📅 [shopper](https://github.com/parthkansal823/shopper) · [Live demo](https://shopper-ap823.netlify.app)
Calendly / Cal.com-style scheduling platform. Hosts publish booking pages, invitees pick a slot and verify their email, and the whole lifecycle — confirmations, reminders, reschedules, cancellations — runs itself, with Google Calendar, Gmail API and webhook integrations. 82 tests in CI; deployed on Netlify + Render.

`React` `FastAPI` `MongoDB Atlas` `Google APIs`

---

## 🧩 More Projects

| Project | What it is | Stack |
|---|---|---|
| **[Adaptive_IAM](https://github.com/parthkansal823/Adaptive_IAM)** | Adaptive identity and access management with risk-based dynamic MFA, LLM-based authorization and blockchain-assisted trust (joint major project) | `Next.js` `FastAPI` `PostgreSQL` `Redis` `Blockchain` |
| **[System Log Analyzer & Anomaly Detector](https://github.com/parthkansal823/System-Log-Analyzer-Anomaly-Detector)** | Real-time log monitor with three anomaly detectors (sliding window, keyword frequency, source burst), file-watch mode and generated reports | `C++17` `OOP` |
| **[Diabetes Prediction](https://github.com/parthkansal823/Diabetes-Prediction-using-Soft-Computing)** | Pima Indians dataset: EDA, missing-value handling, SMOTE for class imbalance and a grid-search-tuned Random Forest (~77% accuracy) | `Python` `scikit-learn` `Jupyter` |

---

## ⚙️ Tech Stack

| Domain | Stack |
|---|---|
| **Languages** | Python · JavaScript · C/C++ · SQL · Java |
| **AI / ML** | PyTorch · scikit-learn · LightGBM · NumPy · Pandas · Jupyter · Gemini API |
| **Backend** | FastAPI · Node.js · Express · REST · WebSockets · WebRTC |
| **Frontend** | React · Next.js · Vite · Tailwind CSS · Recharts · Leaflet |
| **Data** | PostgreSQL · MongoDB · Redis |
| **Tooling & Cloud** | Git · GitHub Actions · Docker · Linux · pytest · Vitest · Netlify · Render |

---

## 🔬 Current Focus

- **ML for systems** — learned query optimization, uncertainty estimation, and knowing when a model should *not* act
- **AI security** — active deception, attack detection, and evaluating defences against LLM-driven attackers
- **LLM systems** — transformers, attention, agents, and practical fine-tuning
- **Engineering fundamentals** — DSA, system design, testing, and shipping end-to-end products

---

I'm looking for high-growth teams building AI-native products and intelligent systems — software that creates measurable value. Say hi at [parth.kansal823@gmail.com](mailto:parth.kansal823@gmail.com).
