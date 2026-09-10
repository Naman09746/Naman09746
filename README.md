<h1 align="center">Hi there, I'm Naman Joshi! 👋</h1>
<h3 align="center">AI / ML + GenAI Engineer | BTech CSE (AI & ML) at K.R. Mangalam University (Expected 2027)</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/naman-joshi0313/">
    <img src="https://img.shields.io/badge/LinkedIn-Naman%20Joshi-blue?style=for-the-badge&logo=linkedin" alt="LinkedIn Badge" />
  </a>
  <a href="mailto:namanjoshi09746@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact%20Me-red?style=for-the-badge&logo=gmail" alt="Email Badge" />
  </a>
  <a href="https://github.com/Naman09746">
    <img src="https://img.shields.io/badge/GitHub-Naman09746-black?style=for-the-badge&logo=github" alt="GitHub Badge" />
  </a>
  <a href="https://leetcode.com/u/namanjoshi09746/">
    <img src="https://img.shields.io/badge/LeetCode-Naman%20Joshi-orange?style=for-the-badge&logo=leetcode" alt="LeetCode Badge" />
  </a>
</p>

---

## 🚀 About Me

- 🎓 **Student:** Pursuing BTech in CSE (AI & ML) at **K.R. Mangalam University** (Expected Graduation: 2027)
- 🎯 **Specialization:** Machine Learning, Generative AI, RAG, and AI Agents
- 🌱 **Currently building:** multi-agent systems, retrieval pipelines, and full-stack AI products
- 🏆 **Certifications:** AWS Solutions Architect | AWS Cloud Practitioner
- 💬 **Ask Me About:** RAG, AI agents, ML systems, and full-stack AI products
- 🤝 **Open to:** Internship opportunities, collaborative projects, and research initiatives
- ⚡ **Languages:** English, Hindi

---

## 🛠️ Technical Skills

### Programming Languages
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white" alt="Java" />
</p>

### AI / ML / GenAI
<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow" />
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-Learn" />
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge" alt="LangGraph" />
  <img src="https://img.shields.io/badge/XGBoost-337AB7?style=for-the-badge" alt="XGBoost" />
</p>

### Backend & Data
<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="SQL" />
</p>

### Frontend & Infra
<p>
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS" />
</p>

---

## 📂 Projects

#### 🔹 **Project 1: Self-Healing RAG**
- **Description:** A closed-loop, multi-agent RAG system that evaluates its own answers, diagnoses retrieval failures, and autonomously repairs weak responses before returning them — instead of the typical retrieve-once, generate-once RAG pipeline.

Key Steps:
- Agent Pipeline: 7-agent LangGraph pipeline (Intake → Planner → Retriever → Generator → Critic → Healer → Output).
- Hybrid Retrieval: Combine ChromaDB dense retrieval, BM25 sparse retrieval, and Neo4j graph retrieval, fused with Reciprocal Rank Fusion and cross-encoder reranking.
- Reliability: Claim-level grounding, hallucination detection, 4-way critic routing (fully supported / partially supported / unsupported / contradicted), prompt-injection detection.
- Self-Healing Loop: On weak grounding, rewrite the query, re-retrieve, re-generate, and re-verify before output.
- Evaluation: Continuous RAGAS-based evaluation of faithfulness, relevancy, and grounding.
- Production Engineering: Auth/RBAC, tenant isolation, rate limiting, Kubernetes deployment, and observability via Prometheus, Grafana, OpenTelemetry, and LangSmith.
- Results (development-stage evaluation): 82% healing success rate, 0.92 answer relevancy, 0.85 context precision, 0.83 grounding score, 2.1s p95 latency.

- **Tech Stack:** Python, LangGraph, FastAPI, Next.js, ChromaDB, Neo4j, PostgreSQL, Redis, Docker, Kubernetes, RAGAS
- **Repository:** [github.com/Naman09746/Self-Healing-RAG](https://github.com/Naman09746/Self-Healing-RAG)

## Project 2: Agentic Marketing Platform

- **Description:** A governed multi-agent decision system where LLM agents generate and evaluate marketing strategies inside a simulated market, using contextual bandits and off-policy evaluation to gate what actually gets deployed. Released as a de-identified thesis project — company-specific data and knowledge base were removed.

Key Steps:
- Agentic Workflow: LangGraph StateGraph covering market observation, strategy optimization, content generation, safety validation, cost checking, simulation, evaluation gating, governance, and canary deployment.
- Optimization: Contextual bandits (LinUCB, Thompson Sampling) evaluated offline with IPS, Direct Method, and Doubly Robust estimation before rollout.
- Simulation: SimPy-based market environment with customer agents, competitor agents, and calibrated personas across Blog, Email, LinkedIn, and X.
- RAG Layer: PostgreSQL + pgvector semantic retrieval with a semantic cache.
- Governance: Human-in-the-loop review, golden-test gates, safety/claim validation, budget enforcement, canary rollout.
- Observability Console: 16-page Streamlit dashboard covering campaigns, experiments, policy evaluation, and deployments.

- **Tech Stack:** Python, LangGraph, FastAPI, PostgreSQL, pgvector, Redis/RQ, Streamlit, MLflow, Prometheus, Grafana, Docker
- **Repository:** [github.com/Naman09746](https://github.com/Naman09746)

## Project 3: Building Ecosystem CRM — CallCRM 2.0

- **Description:** A domain-heavy CRM and sales operating system built around the real-world workflows of India's real-estate industry, architected to extend into the broader building ecosystem (construction, architecture, interiors, materials) over time.

Key Steps:
- Domain Model: Unified data model across People, Property, Inventory, Relationships, Communication, Activities, Deals, Money, Documents, and Operations.
- Event-Driven Automation: CallCRM stays the source of truth; domain events flow through a transactional outbox to n8n via HMAC-SHA256 signed webhooks, with retries and circuit breakers.
- Real-Estate Intelligence: Property hierarchy (Region → Area → Society → Tower → Floor → Unit), mandate engine with seller price floors, negotiation room, site-visit OS, Indian brokerage/GST/TDS engine.
- AI Modules: Seller intelligence, 100-point buyer/inventory matcher, site-visit pre-briefing, lost-lead resurrection, WhatsApp sales engine — with human approval required for sensitive AI-driven changes.
- Testing: 83 routes, 239 tests across 28 test suites, CI pipeline, Supabase Row-Level Security across 39 tables.

- **Tech Stack:** Next.js, React, TypeScript, Tailwind CSS, Supabase, PostgreSQL, Gemini 2.5 Flash, Vercel AI SDK, n8n
- **Repository:** [github.com/Naman09746/Real-Estate-SAAS](https://github.com/Naman09746/Real-Estate-SAAS)

## Project 4: DataGuard

- **Description:** An ML observability platform that turns data-quality issues, distribution drift, and feature/target leakage into actionable, explainable intelligence — so model failures can be traced back to the data before they hit production.

Key Steps:
- Data Quality: Automated checks on uploaded datasets for structural and statistical issues.
- Drift Intelligence: Population Stability Index (PSI) and Kolmogorov-Smirnov tests to detect distribution shifts.
- Leakage Discovery: Feature/target relationship analysis visualized through force-directed graphs.
- AI Insight Engine: Fine-tuned a domain-specific Lily-1.5B model with Unsloth + LoRA to generate natural-language explanations of data-quality issues.
- Async Processing: Heavy statistical computation offloaded to Celery workers with Redis as the broker.
- Health Score: Combines quality, drift, and leakage signals into a single 0–100 integrity score.

- **Tech Stack:** Python, FastAPI, React, TypeScript, PostgreSQL, Celery, Redis, Pandas, SciPy, Scikit-learn, Unsloth, LoRA
- **Repository:** [github.com/Naman09746/data-guard](https://github.com/Naman09746/data-guard)

## Project 5: AI-Powered Vehicle Health Monitoring
- **Description:** A predictive-maintenance platform that converts real-time vehicle telemetry into failure-risk predictions, explainable health scores, and actionable maintenance alerts.

Key Steps:
- Telemetry Ingestion: Handles 10 sensor channels — engine temperature, oil pressure, coolant temperature, RPM, vibration, fuel consumption, battery voltage, tire pressure, speed, and engine load — via CSV upload or MQTT.
- ML Pipeline: Trains and compares five ML classifiers under a champion/challenger model registry with automatic promotion.
- Explainability: SHAP explanations attached to every failure-risk prediction, showing which sensor signals drove it.
- Health Scoring: Composite 0–100 vehicle health score with corresponding health band.
- Application Layer: Fleet overview, vehicle dashboards, alerts, maintenance history, and PDF reporting.

- **Tech Stack:** Next.js, FastAPI, PostgreSQL, Redis, MQTT (Mosquitto), SQLAlchemy, SHAP, Docker, JWT
- **Repository:** [github.com/Naman09746/AI-powered-vehicle-health-monitoring](https://github.com/Naman09746/AI-powered-vehicle-health-monitoring)

## Project 6: NeuroPlan AI

- **Description:** An adaptive study-execution engine that models how a learner is actually progressing and continuously reshapes their study plan using knowledge tracing, spaced repetition, and a fine-tuned language model.

Key Steps:
- Knowledge Tracing: PyTorch-based Deep Knowledge Tracing model estimates the learner's current mastery from performance history.
- Spaced Repetition: Implements a 1–3–7 day review schedule driven by mastery predictions.
- LLM Planning: Locally fine-tuned LLaMA 3.1 8B (QLoRA, packaged as GGUF) generates and adapts study plans.
- Elastic Rescheduling: Missed tasks are redistributed into future lower-density windows instead of simply marked overdue.
- Analytics: Tracks cognitive load, neural efficiency, and knowledge mastery over time.

- **Tech Stack:** Python, PyTorch, LLaMA 3.1 8B, QLoRA, FastAPI, PostgreSQL, React, Zustand, Tailwind
- **Repository:** [github.com/Naman09746/NeuroPlan-AI](https://github.com/Naman09746/NeuroPlan-AI)

## Project 7: Intelligent Microgrid

- **Description:** An AI-driven energy forecasting system that predicts solar generation and household demand to support smarter battery scheduling and peer-to-peer energy trading. Built on a fork of [theabhinav0231/Intelligent-Microgrid](https://github.com/theabhinav0231/Intelligent-Microgrid) — the forecasting work and metrics below are my contribution, not a claim over the full upstream system.

Key Steps:
- Solar Forecasting: XGBoost model trained on 175K rows of NASA POWER data across 5 cities over 5 years.
- Load Forecasting: XGBoost model trained on 3.28M rows across 75 homes over 5 years.
- Feature Engineering: GHI, cell temperature, and power lag for solar; 1-hour and 24-hour load lag plus temperature for demand.
- Application: Forecasts feed a strategic layer for battery scheduling and peer-to-peer energy trading decisions.

- **Results:** Solar forecast — 2.84% MAPE, 0.0088 kW RMSE. Load forecast — 13.95% MAPE, 0.2066 kW RMSE.
- **Tech Stack:** Python, XGBoost, NASA POWER data, PVLib
- **Repository:** [github.com/Naman09746/Intelligent-Microgrid](https://github.com/Naman09746/Intelligent-Microgrid)

---

## 📊 GitHub Stats & Activity
<p align="center">
  <img width="48%" src="https://github-readme-stats.vercel.app/api?username=Naman09746&show_icons=true&theme=tokyonight" alt="GitHub Stats" />
  <img width="48%" src="https://github-readme-streak-stats.herokuapp.com/?user=Naman09746&theme=tokyonight" alt="GitHub Streak" />
</p>

---

## 🤝 Let's Connect!
- **Email:** [namanjoshi09746@gmail.com](mailto:namanjoshi09746@gmail.com)
- **LinkedIn:** [linkedin.com/in/naman-joshi0313](https://www.linkedin.com/in/naman-joshi0313/)
- **GitHub:** [github.com/Naman09746](https://github.com/Naman09746)
- **LeetCode:** [leetcode.com/u/namanjoshi09746](https://leetcode.com/u/namanjoshi09746/)

> *Build systems, not demos.*

---

*Thank you for visiting my profile. Let's create, innovate, and inspire together!*
