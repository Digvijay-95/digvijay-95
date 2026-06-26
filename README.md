<h1 align="center">Hi there, I'm Digvijay Mahamuni 👋</h1>
<h3 align="center">Backend Engineer | AI & LLM Systems</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/digvijay95"><img src="https://img.shields.io/badge/-LinkedIn-blue?style=flat&logo=Linkedin&logoColor=white"/></a>
  <a href="mailto:mahamunidigvijay@gmail.com"><img src="https://img.shields.io/badge/-Email-red?style=flat&logo=Gmail&logoColor=white"/></a>
  <a href="https://leetcode.com/u/Digvijay95/"><img src="https://img.shields.io/badge/-LeetCode-orange?style=flat&logo=LeetCode&logoColor=white"/></a>
</p>

---

### 🧑‍💻 About Me

- 🔧 Backend Engineer focused on distributed systems, container orchestration, and AI/LLM-powered platforms.
- 🛡️ Like understanding systems from the inside — I'd rather hand-roll the Kubernetes mechanics than reach for a fully managed abstraction.
- 🤖 Deep interest in AI/LLM systems — RAG, agentic workflows, MCP, and local inference with Ollama.
- 🌱 Currently deep in container orchestration internals — session lifecycles, Pod-level isolation, and idle-resource reaping.

---

### 🚀 Featured Project: MCP Session Orchestrator

A from-scratch container orchestration framework for dynamically provisioning isolated, ephemeral runtime environments for **MCP (Model Context Protocol)** tool servers — built end-to-end without abstracting away the Kubernetes mechanics.

**Core design:**
- Shared Kubernetes namespace with **Pod-per-(session × selected MCP server)**, instead of a heavier namespace-per-session model.
- Session-scoped `NetworkPolicy`, keyed by a `session-id` label, replacing full namespace-level isolation.
- **Redis-backed session registry** with idle-TTL reaping — active sessions get instant routing, idle ones get cleaned up automatically.
- Readiness checks built on a real MCP `initialize` handshake over streamable HTTP, not just "container is Running."
- Direct Pod-IP routing for tool calls — no Kubernetes Service objects needed.
- Structured JSON logging, correlated by session ID across the full provision → serve → reap lifecycle.

**Stack:** Python, FastAPI, Kubernetes Python client / `kr8s`, `redis-py` (async), `httpx` (async), `structlog`, k3s/kind + Calico for local development.

*Status: actively building.*

---

### 🛠️ Tech Stack

**Languages & Frameworks**

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat&logo=fastapi&logoColor=white)

**Cloud & Infrastructure**

![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat&logo=amazon-aws&logoColor=white)
![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat&logo=docker&logoColor=white)
![NGINX](https://img.shields.io/badge/-NGINX-009639?style=flat&logo=nginx&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat&logo=linux&logoColor=black)

**Databases**

![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/-Redis-DC382D?style=flat&logo=redis&logoColor=white)

**AI / LLM**

![LangChain](https://img.shields.io/badge/-LangChain-1C3C3C?style=flat)
![LangGraph](https://img.shields.io/badge/-LangGraph-1C3C3C?style=flat)
![Ollama](https://img.shields.io/badge/-Ollama-000000?style=flat)
![MCP](https://img.shields.io/badge/-Model%20Context%20Protocol-6E56CF?style=flat)

---

### 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Digvijay-95&show_icons=true&theme=tokyonight" alt="Digvijay's GitHub Stats" height="170"/>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Digvijay-95&theme=tokyonight" alt="GitHub Streak" height="170"/>
</p>

---

### 📫 Connect With Me

- 💼 LinkedIn: [linkedin.com/in/digvijay95](https://www.linkedin.com/in/digvijay95)
- 💻 LeetCode: [leetcode.com/u/Digvijay95](https://leetcode.com/u/Digvijay95/)
- 📧 Email: mahamunidigvijay@gmail.com

---

<p align="center"><i>Backend systems, AI agents, and a healthy curiosity about how things work under the hood.</i></p>
