# Hi, I'm Sheryar Ahmed 👋

**Full-Stack Engineer** who builds *and operates* production systems end to end — schema, API, frontend, deploy, and on-call.

4+ years across SaaS, healthcare, real-time streaming, and marketplaces. Creator and lead engineer of **Pathment** — open-source mentorship infrastructure for enterprise teams: **3,000+ active users, 18 contributors, 500+ production deployments.**

🌐 [Portfolio](https://sheryarahmed.netlify.app) · 🚀 [Pathment (live)](https://pathment.me) · 💼 [LinkedIn](https://linkedin.com/in/sheryar-ahmed) · 📺 [YouTube](https://www.youtube.com/@sheryarsystems)

---

## 🧩 What I'm building

### [Pathment](https://pathment.me) — Creator & Lead Engineer
Open-source mentorship infrastructure for enterprise teams. Sole engineer through design, build, and launch; now maintained with **18 contributors**, one funded through Dev Weekends Summer of Code.

- **BYOK AI** — roadmap generation against any OpenAI-compatible provider (Groq, OpenAI, Anthropic, OpenRouter). Customers bring their own key, so the model can't be assumed good: output passes JSON schema validation, multi-stage sanitization, and a repair pass before reaching the UI. Keys encrypted at rest, never logged.
- **Postgres-backed email queue** at a 500K emails/month budget with no Redis or Bull — `FOR UPDATE SKIP LOCKED`, exponential backoff with jitter, dead-letter, idempotency keys, suppression list, and priority lanes so a password reset never queues behind a bulk campaign.
- **Self-hosted live video** — embedded Jitsi (prosody / jicofo / JVB) for cohort reviews, attendance derived from join/leave events, contribution scored from talk time, zero media stored.
- **Scoped RBAC** — org → program → clan → self, with a permission catalog, derived capabilities, role delegation, and full audit logging, resolved in one place rather than per controller.
- **Modular monolith by choice** — 11 bounded domains in one Postgres database, with a documented split plan for when traffic justifies services. Onboarding docs get a new contributor shipping in their first week.
- **Ops** — 500+ deployments on a zero-downtime expand–migrate–deploy runbook. Docker, Caddy (auto-TLS), GitHub Actions CI/CD across staging and production.

---

## 🚀 Featured Projects

### [Ticketing Microservices Web App](https://github.com/Sheryar-Ahmed/ticketing-microservices-web-app)
StubHub-style marketplace built as **6 event-driven microservices** (Next.js, NATS, MongoDB, Redis, Bull, Stripe, Kubernetes). Shared TypeScript package for type-safe event contracts, optimistic concurrency control for out-of-order events, crash-safe replay via durable NATS subscriptions.

### [MERN CI/CD on AWS](https://github.com/Sheryar-Ahmed/mern-cicd-aws)
Automated deployment pipeline — GitHub Actions, Docker, AWS.

---

## 📺 Teaching

- **Cloud & DevOps series (Dev Weekends)** — 8-part AWS series taken from my own production setups. [https://youtube.com/playlist?list=PL_yEmchnldCPbxySt5lOA-aUvSAYDMQN4&si=rWeeqrGojVZ-gryo]
- **Observability from first principles** — deep-dive walkthrough of OpenTelemetry, Prometheus, Grafana, Loki, and Tempo on a real system. [https://youtu.be/tWpm8iP1AHU?si=2Pqr-GjVGMl4XxmA]
- Mentor developers through **Dev Weekends**.

---

## 🔬 Currently going deep on

PostgreSQL internals, hands-on — reproducing behaviour in a lab, not reading about it:
- Isolation levels & MVCC — why Postgres has no dirty reads and no phantoms at REPEATABLE READ, and what SERIALIZABLE forces your application to build
- Locks & deadlocks — caused a 40P01 on purpose, fixed it with lock ordering, and learned to find the blocker (not the victim) in `pg_stat_activity`

---

## 💼 Experience

**TechWinture** (Germany · Remote) — Full-Stack Engineer · *Oct 2025 – Present*
- *PACK (Azure SaaS on Microsoft Marketplace):* transactable offers, always-on webhook on Azure Container Apps, Teams media bot, Entra ID admin-consent flows; migrated the FastAPI service from hexagonal to modular architecture
- *Raumdeuter (fan engagement):* SSE + Redis Pub/Sub multi-instance real-time; dashboard load cut from 6–8s to sub-second

**Appsologix** — Full-Stack Engineer · *Jun 2024 – Sep 2025*
- Peepskill (2,000+ users), HealthSIA (7-role RBAC healthcare), Royal Vision (booking + payments on GCP)

**Freelance** — Full-Stack Developer · *Sep 2022 – Jun 2024*
- Pixy Live (live streaming: agency system, virtual gift economy), Oqvest (US mortgage platform: workflows, Playwright automation, AWS + Docker CI/CD), Doorcut (barber marketplace, React Native)

**Z2A Tech** — Frontend Engineer · *Sep 2021 – Sep 2022*

---

## 🛠️ Tech Stack

**Languages:** TypeScript, JavaScript, Python
**Backend:** Node.js, Express, FastAPI, REST, GraphQL
**Frontend:** React, Next.js, React Native, Tailwind CSS, Redux
**Databases:** PostgreSQL (MVCC, isolation levels, locking, `SKIP LOCKED` queues), MySQL, MongoDB, Redis
**Real-time & Messaging:** Socket.IO, WebSockets, SSE, NATS, Kafka, Bull
**AI / LLM:** BYOK integrations across OpenAI-compatible providers, RAG, structured output with validation + repair passes
**Observability:** OpenTelemetry, Prometheus, Grafana, Loki, Tempo
**DevOps & Cloud:** Docker, Kubernetes, GitHub Actions, AWS, Azure (Container Apps, Entra ID), GCP, Caddy, Nginx

---

## 📫 Contact

- **LinkedIn:** https://linkedin.com/in/sheryar-ahmed
- **Portfolio:** https://sheryarahmed.netlify.app
- **Pathment:** https://pathment.me
- **Email:** royalsheryar505@gmail.com
