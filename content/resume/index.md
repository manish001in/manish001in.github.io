+++
date = "2026-10-27"
+++

# Manish Rastogi - Resume

**Senior Software Engineer — Backend & AI Systems**  
📍 Bengaluru, India  
📧 [manish.rastogi94@gmail.com](mailto:manish.rastogi94@gmail.com)  
[GitHub](https://github.com/manish001in) | [LinkedIn](https://www.linkedin.com/in/manish--rastogi)

[📄 **Download PDF Resume**](/files/resume.pdf)

---

## 🧠 Professional Summary

Backend and AI engineer with **10+ years** of experience building systems end to end — from low-latency trading platforms to **LLM agents in production**. Most recently built the provider-agnostic tool-calling architecture and the full integration layer for an AI assistant, plus the evals that measured whether the agents actually worked. Comfortable owning a problem from architecture through on-call, have led teams of up to ~10, and spent two years founding my own product — so I bias toward shipping and cost, not just design docs.

---

## 💼 Experience

### 🐦 **Senior Software Engineer – Studio Management (Littlebird)**
*August 2025 – July 2026 · Bengaluru*

Littlebird is an AI executive assistant (grew from 250 to 5,000 users). Also built Songbird, a music-recommendation product.

- Rebuilt the agent's core tool-calling loop into a **provider-agnostic plugin system** (OpenAI Responses + Gemini) with per-turn tool management — the pattern other engineers then built their own agents on.
- Owned the **integrations layer** end to end, backend through UI: Composio and OAuth with per-tool routing on the backend, plus the toggle wired across the client SDK, stores, and UI — connecting 8 platforms (Gmail, Drive, Docs, Sheets, Calendar, Linear, GitHub, Notion).
- Built the **evaluation framework** (judge prompts and datasets) for the main agent and subagents, raising integration eval scores from **64% to 85%+** and catching regressions before release.
- Built the meeting-notes backend: turned in-app meeting transcripts into cleanly formatted notes with speaker handling, and matched Google Calendar events to the meetings a user started so each note attached to the right meeting.
- Drove Google's **CASA security certification** end to end — the review required for production access to users' Gmail, Drive, and Calendar data.
- Added the reliability and observability behind it: usage and error telemetry with dashboards, plus handling for dropped connections and interrupted model streams.

**🎵 Songbird — solo build (music recommendation)**

- Designed and built the entire platform alone — data pipeline, infrastructure on Modal, and the recommendation modeling.
- Modeled each user's taste from their listening history: enriched every track with LLM calls (Gemini with search grounding) and audio features, turned them into embeddings, then reduced dimensions two ways as Modal jobs — unsupervised (PCA) to visualize a library, and supervised (PLS) aligned to the user's own likes and dislikes.
- Built a preference model that scores each song's appeal from ~100 pieces of feedback (hearts, thumbs, ranked comparisons), calibrated so its head-to-head predictions stay honest — refreshing as new ratings arrive and driving what gets recommended next.
- Re-architected from Spotify-only to provider-agnostic, adding Apple Music behind the same interface.

---

### 🛠️ **Software Engineer (Contract) – Docsum**
*February 2025 – June 2025 · Bengaluru*

- Built the async task system (an async-tasks table with a streaming status endpoint) powering bulk document operations — bulk archive and bulk reprocess — across high-volume workloads.
- Built the document-relationship layer: new relationship tables plus a bulk endpoint that computes relationships across many documents at once, forming the backbone of the inter-document knowledge graph (pgRouting + LLMs).
- Built the Google Drive integration (Paragon workflows) and file-sync APIs for bringing external documents in.
- Hardened the FastAPI / SQLAlchemy backend: fixed dependency-injection and DB-session bugs, file-type detection, and persistence issues.

**Tech Stack:** Python, FastAPI, SQLAlchemy, Hatchet, PostgreSQL

---

### 🧪 **Founder – Twing** ([https://trytwing.com](https://trytwing.com))
*December 2022 – January 2025 · India*

Solo-founded an AI productivity startup; built and shipped four products.

- **TwingBot**: AI Slack bot for task management; ~200 users, saving 30+ minutes a day.
- **Legaling**: RAG-based legal research and case management (Azure Vector DB, OpenAI, Search Service).
- **TwingParse**: Template-based extraction from varied documents using OCR and language detection.
- **TwingTranslate**: Translation for Indian languages across scanned and digital documents.

**Tech Stack:** Python, FastAPI, PostgreSQL, Celery, AWS, Azure, LlamaIndex, LangChain

---

### 🚀 **Technical Lead – Salarybox**
*April 2022 – July 2022 · Gurugram*

- Built a real-time notification engine from scratch that scaled to **3,000 notifications/min** for thousands of simultaneous users, using Redis, queues, and batching over a dynamic rule set.
- Cut latency from **30s to 1–2s** and DB locks from ~300 to 2–5 per day by fixing several problem processes; added monitoring and the ability to re-run requests in testing.
- Cut AWS and infrastructure spend **~30%** by moving to ARM servers and rightsizing after performance tests.
- Led and mentored a team of 6.

**Tech Stack:** Python, Django, Redis, PostgreSQL, Celery, AWS

---

### 💼 **Senior Software Engineer – Instawork**
*October 2021 – April 2022*

- Built the tipping feature (multiple touchpoints, rating-based calculation) that raised client tipping by up to **15%**.
- Added fraud-detection checks that analyzed tipping behavior against expected parameters.

**Tech Stack:** Python, Django, JavaScript

---

### 📊 **Software Developer – Quadeye Securities**
*February 2017 – December 2020 · Gurgaon*

- Architected a low-latency trading-visualization app handling up to **3,000 data points/second**, with live alerts and commands into trading strategies.
- Drove ~5x throughput gains — websockets, Redis caching, and queue-based offloading — taking capacity from **5k to 1M events/day**.
- Helped hire and manage a team of 10+.

**Tech Stack:** Python, Django, jQuery, JavaScript, MySQL, Redis

---

### 💻 **Software Developer – Ishi Systems**
*December 2015 – January 2017 · Ahmedabad*

- Built on-the-fly video processing (Intel Media SDK, Go), made systems ONVIF-compliant, and worked full-stack across Python / Django and AngularJS.

---

## 🧩 Projects

### 📜 **Clausewize** ([clausewize.app](https://clausewize.app) · solo)

A Chrome extension that turns terms-of-service and privacy pages (and PDFs) into a plain risk brief: a verdict, severity-rated clauses, and the exact clause each flag came from. Bring-your-own-key across OpenAI, Anthropic, and Gemini; privacy-first (stores no raw documents); with an account tier for synced history and shareable briefs. Live on the Chrome Web Store.

### 🔔 **Pushbridge** ([GitHub](https://github.com/manish001in/pushbridge) · open source, 18★)

A Manifest V3 Chrome extension that rebuilds core Pushbullet features (notification mirroring, SMS/MMS, push and file sync) on the official REST and WebSocket APIs. TypeScript + Lit, unit and end-to-end tested, 12 releases. The hard part: keeping a live WebSocket sync working under MV3's short-lived service worker.

---

## 🧠 Technical Skill Set

### 💻 Languages  
Python, JavaScript / TypeScript, Go

### ⚙️ Backend  
Django, FastAPI, Flask, Node.js

### 🧠 AI / LLM  
Tool-calling agents, evals, embeddings & retrieval, RAG · OpenAI, Anthropic, Gemini · LlamaIndex, LangGraph

### ☁️ Data & Infra  
PostgreSQL, MySQL, Redis, Supabase · AWS (EC2, ECS, S3, Lambda, RDS), Modal, Docker, GitHub CI

---

## 🎓 Education

**Nirma University**  
Bachelor of Technology (B.Tech) – Information Technology  
*2012 – 2016*

---

*Last updated: July 2026*
