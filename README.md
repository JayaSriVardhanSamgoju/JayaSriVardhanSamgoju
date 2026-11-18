<!-- ======================= HEADER ======================= -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:1F6FEB,100:58A6FF&height=220&section=header&text=Jaya%20Sri%20Vardhan%20Samgoju&fontSize=40&fontColor=ffffff&fontAlignY=38&desc=AI%20%26%20Full-Stack%20Engineer%20%7C%20LLM%20Systems%20%7C%20Agentic%20RAG&descAlignY=58&descSize=17" width="100%"/>

<a href="https://github.com/JayaSriVardhanSamgoju">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3200&pause=1000&color=58A6FF&center=true&vCenter=true&width=760&lines=Building+evidence-driven+AI+systems;Agentic+RAG+%C2%B7+LangGraph+%C2%B7+FastAPI+%C2%B7+React;From+idea+to+validated+product%2C+end+to+end" alt="Typing animation"/>
</a>

<br/>

<a href="https://www.linkedin.com/in/jaya-sri-vardhan-samgoju"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
<a href="mailto:srivardhansamgoju@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-EA4335?style=flat-square&logo=gmail&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Open%20to-Internships%20%26%20Entry--Level%20Roles-2EA043?style=flat-square"/>
<img src="https://komarev.com/ghpvc/?username=JayaSriVardhanSamgoju&label=Profile%20Views&color=1F6FEB&style=flat-square"/>

</div>

---

## 👨‍💻 About

I am a **Computer Science undergraduate** who builds **full-stack and AI-powered products**. I like taking an unclear problem and owning it from the first line of code to final validation.

My work focuses on **backend APIs, real-time systems, LLM agents and retrieval pipelines**, with a strong habit of testing, tracing and measuring what I build.

| | |
|:--|:--|
| 🎓 **Education** | B.Tech in Computer Science & Engineering, **RGUKT Ongole** (2023 – 2027) · **CGPA 9.1 / 10** |
| 📍 **Location** | Ongole, Andhra Pradesh, India 🇮🇳 |
| 🔭 **Focus** | Agentic AI · RAG · LLM reliability · Production backends |
| 🎯 **Looking for** | ML / AI / Full-Stack internships and entry-level roles |
| 📫 **Reach me** | [srivardhansamgoju@gmail.com](mailto:srivardhansamgoju@gmail.com) |

---

## 🚀 Featured Projects

### 🔎 [IncidentLens](https://github.com/JayaSriVardhanSamgoju/IncidentLens) — Evidence-Driven Incident Investigation Platform

> An AI platform that helps operators find the root cause of an incident, using evidence from logs, metrics, deployments and past incidents. Every finding keeps its source, so nothing is a black box.

<img src="https://skillicons.dev/icons?i=fastapi,react,ts,vite,postgres,docker&theme=dark" alt="IncidentLens stack"/>

**What it does**
- Full-stack app: **React + TypeScript** frontend, **FastAPI** REST APIs, and **Server-Sent Events (SSE)** for live updates.
- A stateful **LangGraph** workflow that mixes rule-based root-cause analysis with **5 specialist agents**: logs, metrics, deployments, service dependencies and historical incidents.
- Keeps **evidence provenance** and shows **conflicting findings** instead of hiding them.
- **Human-in-the-loop** review: `APPROVE`, `REJECT` or `REQUEST MORE EVIDENCE`.
- Live timeline with **SSE reconnect and event replay**, typed API clients and system health monitoring.

| Tests passed | End-to-end scenarios | Specialist agents |
|:--:|:--:|:--:|
| **312 / 312** | **15 / 15** | **5** |

```mermaid
flowchart LR
    UI["React + TypeScript UI"] -->|"REST + SSE"| API["FastAPI"]
    API --> G["LangGraph Orchestrator"]
    G --> A1["Logs Agent"]
    G --> A2["Metrics Agent"]
    G --> A3["Deployments Agent"]
    G --> A4["Dependencies Agent"]
    G --> A5["History Agent"]
    A1 & A2 & A3 & A4 & A5 --> H["Ranked Hypotheses"]
    H --> R["Human Review: Approve / Reject / More Evidence"]
    API <--> DB[("PostgreSQL")]
```

---

### 📚 [SynoptiQ](https://github.com/JayaSriVardhanSamgoju/SynoptiQ) — Enterprise Agentic RAG & Document Intelligence Platform

> Ask questions about your documents and get answers backed by evidence, with **page-level citations** so you can check every claim.

<img src="https://skillicons.dev/icons?i=fastapi,nextjs,postgres,redis,docker&theme=dark" alt="SynoptiQ stack"/>

**What it does**
- Multi-format document ingestion, hybrid retrieval, grounded answers and **page-level citation tracing**.
- **LangGraph multi-agent pipeline:** query planning → hybrid retrieval → synthesis → verification.
- **High-precision retrieval:** dense vector search + **BM25** + **Reciprocal Rank Fusion** + **HyDE** + **cross-encoder reranking**.
- **Defense-in-depth security:** input, context and output guardrails for prompt injection, jailbreaks, PII, API-key leaks, indirect context poisoning and system-prompt leakage, with security evaluation and regression tests.
- **Production-ready upgrades:** PostgreSQL + **pgvector**, Redis-backed ephemeral BYOK sessions, async document workers, semantic chunking, **OpenTelemetry** tracing, automated RAG evaluation and CI/CD checks.

```mermaid
flowchart LR
    D["Documents"] --> I["Ingest + Semantic Chunking"]
    I --> V[("pgvector + BM25 Index")]
    Q["User Question"] --> P["Query Planner"]
    P --> H["Hybrid Retrieval: Dense + BM25 + RRF + HyDE"]
    V --> H
    H --> X["Cross-Encoder Rerank"]
    X --> S["Synthesis"]
    S --> C["Verification"]
    C --> O["Cited Answer"]
    GR["Guardrails: Input / Context / Output"] -.-> P
    GR -.-> S
    GR -.-> O
```

---

## 🛠️ Tech Stack

<table>
<tr>
<td width="190"><b>💻 Languages</b></td>
<td>
<img src="https://skillicons.dev/icons?i=py,java,cpp,c,ts,postgres&theme=dark" alt="Languages"/>
</td>
</tr>
<tr>
<td><b>⚙️ Backend & Data</b></td>
<td>
<img src="https://skillicons.dev/icons?i=fastapi,flask,postgres,redis&theme=dark" alt="Backend"/>
<br/><sub>REST APIs · SQLAlchemy · SSE · pgvector</sub>
</td>
</tr>
<tr>
<td><b>🎨 Frontend</b></td>
<td>
<img src="https://skillicons.dev/icons?i=react,ts,vite,nextjs&theme=dark" alt="Frontend"/>
</td>
</tr>
<tr>
<td><b>☁️ Cloud & DevOps</b></td>
<td>
<img src="https://skillicons.dev/icons?i=aws,docker,kubernetes,git,github,prometheus,grafana&theme=dark" alt="Cloud and DevOps"/>
<br/><sub>CI/CD · OpenTelemetry · Monitoring</sub>
</td>
</tr>
<tr>
<td><b>🧠 AI / ML</b></td>
<td>
<img src="https://skillicons.dev/icons?i=pytorch,tensorflow,sklearn&theme=dark" alt="ML"/>
<br/><sub>LLMs · RAG · Agentic AI · LangChain · LangGraph · XGBoost</sub>
</td>
</tr>
<tr>
<td><b>🔍 Retrieval & NLP</b></td>
<td>
<img src="https://img.shields.io/badge/FAISS-0467DF?style=flat-square"/>
<img src="https://img.shields.io/badge/BM25-444?style=flat-square"/>
<img src="https://img.shields.io/badge/Embeddings-6E40C9?style=flat-square"/>
<img src="https://img.shields.io/badge/Vector%20Search-1F6FEB?style=flat-square"/>
<img src="https://img.shields.io/badge/Cross--Encoder%20Reranking-2EA043?style=flat-square"/>
<img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black"/>
</td>
</tr>
</table>

---

## 📊 GitHub Activity

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=JayaSriVardhanSamgoju&show_icons=true&theme=github_dark&hide_border=true&count_private=true&bg_color=0D1117" alt="GitHub stats"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=JayaSriVardhanSamgoju&layout=compact&theme=github_dark&hide_border=true&bg_color=0D1117" alt="Top languages"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=JayaSriVardhanSamgoju&theme=github-compact&hide_border=true&bg_color=0D1117&color=58A6FF&line=1F6FEB&point=FFFFFF" alt="Contribution graph" width="95%"/>

</div>

---

## 🏆 Achievements & Certifications

- 🥇 **Top 4 team**, KL University Hyderabad Hackathon, for a **GST Reconciliation** solution that improves financial data validation pipelines.
- 🎓 **NPTEL Elite**: Foundations of Deep Learning (**81%**), an IIT-backed MOOC.
- 🚀 **Ignite India Entrepreneurship Program**, Wadhwani Foundation.

---

## 🧭 How I Work

| Principle | What it means |
|:--|:--|
| **Evidence first** | Every answer or finding should point back to its source. |
| **Test everything** | Automated tests, end-to-end checks and evaluation before I call something done. |
| **Safe by design** | Guardrails, human review and observability are part of the build, not an afterthought. |
| **Own the whole thing** | Design, backend, frontend, deployment and validation. |

---

## 🎯 Currently

- 🔨 Improving **SynoptiQ** toward production-scale (reliability, tracing, evaluation)
- 📖 Studying **LLM reliability** and ways to reduce hallucinations
- 🧪 Practising **DSA** and strengthening core fundamentals
- 🎓 Final year B.Tech · Expected graduation **May 2027**

---

## 🤝 Let's Connect

<div align="center">

<a href="https://www.linkedin.com/in/jaya-sri-vardhan-samgoju"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:srivardhansamgoju@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://github.com/JayaSriVardhanSamgoju"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>

<br/><br/>

<sub>If you like my work, a ⭐ on my repositories is always appreciated.</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:1F6FEB,100:58A6FF&height=110&section=footer" width="100%"/>

</div>
