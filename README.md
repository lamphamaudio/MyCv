<div align="center">

# PHAM THANH LAM

**AI Engineer | Backend Developer (LLM Applications, Agentic Systems)**

Thanh Xuan, Ha Noi &nbsp;|&nbsp; 0394287315 &nbsp;|&nbsp; lamphamaudio@gmail.com
[linkedin.com/in/thanh-lam-phạm-327039236](https://www.linkedin.com/in/thanh-lam-ph%E1%BA%A1m-327039236/) &nbsp;|&nbsp; [github.com/lamphamaudio](https://github.com/lamphamaudio)

</div>

---

## PROFESSIONAL SUMMARY

Backend developer with 2+ years of experience building production REST APIs (.NET 8, Spring Boot, Go), now focused on LLM-powered applications. Built a Vietnamese personal-finance AI assistant (LangGraph agent, function calling, guardrails, human-in-the-loop confirmation, long-term memory, automated evaluation) and a RAG assistant for Discord communities on pgvector. Strong foundation in Clean Architecture, PostgreSQL/SQL Server, Redis, authentication and observability, applied to shipping reliable, safe AI features.

---

## EDUCATION

**Thuy Loi University** — *Bachelor of Information Technology* &nbsp;·&nbsp; Ha Noi &nbsp;·&nbsp; **2021 – 2025**

---

## WORK EXPERIENCE

### VSF &nbsp;·&nbsp; 05/2026 – Present
*AI / Backend Engineer (Probation) — Ha Noi*

- Built **Spectra**, a Vietnamese personal-finance AI assistant: a LangGraph agent with function calling, guardrails, long-term memory and an automated evaluation pipeline.
- Developing **PaySplit**, an AI OCR bill-splitting and settlement fintech app: Redis-backed session auth, SePay bank-transfer settlement and realtime group sync (SSE).
- Worked with spec-driven development, pull-request code reviews and AI-assisted engineering workflows (Claude Code).

### Zamiga &nbsp;·&nbsp; 05/2025 – 03/2026
*Back-End Developer — Ha Noi*

- Designed and implemented scalable RESTful APIs using .NET 8 following Clean Architecture principles.
- Developed dynamic reporting and dashboard modules with Excel import/export integration.
- Optimized complex SQL queries to improve response time and data processing performance.
- Implemented JWT-based authentication and role-based authorization for secure API access.
- Collaborated in Agile teams (sprint planning, code reviews, daily stand-ups).

### SFT Global &nbsp;·&nbsp; 05/2024 – 04/2025
*Backend-Focused Fullstack Developer (Intern → Developer) — Ha Noi*

- Built and maintained RESTful APIs using .NET and Spring Boot.
- Integrated Elasticsearch for real-time document search and indexing.
- Developed document processing features including watermark integration for content protection.
- Designed and optimized SQL queries for high-performance data retrieval; built Vue.js modules on top of these APIs.

---

## AI PROJECT EXPERIENCE

### Spectra – Personal Finance AI Assistant &nbsp;·&nbsp; 05/2026 – 06/2026
*AI Engineer / Main Developer (team of 2, VSF) — [github.com/lamphamaudio/personal-finance-ai-assistant](https://github.com/lamphamaudio/personal-finance-ai-assistant)*

***Technologies:** Python, FastAPI, LangGraph, OpenAI / Gemini, PostgreSQL (Supabase), React + Vite, LangSmith, OpenTelemetry, pytest, Docker*

- **Agent orchestration:** Built a Vietnamese financial chatbot as a LangGraph state machine — guard, planner, tool executor, synthesis and output check — with conditional routing, multi-intent handling and clarification flows.
- **Tool calling:** Designed the function-calling tool layer (spending analysis, budgets, savings goals, anomaly explanation, balance forecast, financial health score) so every answer is grounded in real transaction data.
- **Safety:** Layered guardrails for prompt injection, out-of-scope and investment-advice requests, tool-argument validation and PII redaction on output; write actions require user confirmation and are audited.
- **Memory:** Long-term user memory (preferences, category rules learned from corrections) with sensitive-data filtering, plus persistent chat sessions.
- **Evaluation:** Built an automated evaluation pipeline covering intent classification, tool selection, confirmation flow and answer quality via LLM-as-a-Judge, run as a regression suite alongside unit tests.
- **Observability:** Hierarchical tracing and structured logging for LLM and tool calls (LangSmith, OpenTelemetry) with payload redaction; migrated storage to Supabase Postgres and built a Bank Simulator service with SSO login.

### KingModerator (A20) – RAG Assistant for Discord Communities &nbsp;·&nbsp; 04/2026 – 05/2026
*Fullstack AI Developer (team of 3) — [github.com/lamphamaudio/A20-App-131](https://github.com/lamphamaudio/A20-App-131)*

***Technologies:** Python, FastAPI, PostgreSQL + pgvector, OpenAI, RAG, discord.py, React + TypeScript + Vite, Alembic, Braintrust, Docker*

- Knowledge-first moderation platform: documents are uploaded, reviewed and published as knowledge-base versions, and the Discord bot may only answer from the active version — keeping replies grounded and rollback-able.
- Built the RAG retrieval path: document ingestion and semantic chunking with overlap, embeddings in pgvector, and grounded answer generation with source tracing per chunk.
- Implemented a hybrid content guard (regex first, LLM classifier second, behind a feature flag for cost control) detecting toxic, spam, off-topic and prompt-injection messages, with a moderation queue and remote message deletion on Discord.
- Built the help-center assistant end to end (article models, backend agent, admin UI, chat drawer) and covered its guardrails with tests.
- Developed the moderator dashboard in React/TypeScript: moderation queue, retrieval traces, AI suggestions, reply templates and markdown reply previews; fixed CSRF handling and session caching in authentication.

### PaySplit – AI Bill Splitting & Settlement App &nbsp;·&nbsp; 08/2026 – 09/2026
*Backend & Mobile Developer (team of 3, VSF) — [github.com/FintechVSF-Tranning](https://github.com/FintechVSF-Tranning)*

***Technologies:** Go, chi, PostgreSQL, sqlc, Redis, River queue, SSE, LlamaExtract OCR, VietQR, SePay, Firebase FCM, Flutter (Riverpod, Dio), Docker, Caddy*

- Mobile fintech app that scans receipts with AI OCR, splits items (VAT, fees, discounts) among group members and settles debts through dynamic VietQR payments.
- Contributed to the bill module around the asynchronous OCR worker (receipt → LLM extraction → normalized items) and fixed item-level discount allocation and rounding edge cases in the split engine.
- Replaced JWT + Postgres sessions with opaque credentials backed by Redis (instant revocation, role cache, eviction-policy handling) and wrote the design rationale document.
- Built automatic bank-transfer settlement via SePay webhooks that matches incoming transactions to debts, and a realtime group sync over Server-Sent Events with delta catch-up.
- Implemented group management, pagination and debt-reminder APIs; built Flutter group hub, settlement and authentication screens on a feature-first Clean Architecture.

---

## OTHER PROJECT EXPERIENCE

### CQS &nbsp;·&nbsp; 2025 – 2026
*Back-End Developer*

***Technologies:** .NET 8, .NET Framework 4.7, SQL Server, OpenID Connect (OIDC)*

- Designed centralized authentication with OpenID Connect for Single Sign-On and secure role-based authorization.
- Integrated legacy .NET Framework 4.7 modules into the .NET 8 ecosystem; ensured transactional consistency in SQL Server.

### Legacy System Migration – .NET 4.7.2 to .NET 8 &nbsp;·&nbsp; 2025 – 2026
*Backend Developer*

***Technologies:** .NET 8, .NET Framework 4.7.2, SQL Server*

- Migrated a legacy application to .NET 8 with Clean Architecture; updated DI, middleware and authentication while keeping backward compatibility during rollout.

### Document Management System &nbsp;·&nbsp; 06/2024 – 10/2024
*Backend Developer*

***Technologies:** .NET 8, SQL Server*

- Designed document lifecycle APIs (view, download, print, watermark).

### SMS Service System &nbsp;·&nbsp; 11/2024 – 02/2025
*Backend Developer*

***Technologies:** Spring Boot, SQL Server, Angular*

- Designed message storage by customer type; built bulk Excel upload and secured image upload/download APIs.

---

## TECHNICAL SKILLS

- **AI / LLM:** LangGraph, RAG (chunking, embeddings, pgvector), OpenAI & Gemini APIs, function/tool calling, prompt engineering, guardrails & PII redaction, agent memory, LLM-as-a-Judge evaluation, LangSmith, OpenTelemetry, OCR (LlamaExtract), scikit-learn
- **Languages:** Python, C#, Go, Java, JavaScript, Dart
- **Backend:** FastAPI, .NET 8 / ASP.NET Core, Spring Boot, Go (chi), RESTful API, SSE, Clean Architecture, OIDC / JWT
- **Data & Infra:** PostgreSQL (Supabase), SQL Server, Redis, MySQL, Firebase, Docker, background job queues
- **Mobile:** Flutter
- **Tools:** Git, GitHub, GitLab, SVN, Postman, Visual Studio / VS Code, Claude Code, Figma, Draw.io
- **Languages spoken:** Vietnamese (native), English (reading and writing technical documents)
