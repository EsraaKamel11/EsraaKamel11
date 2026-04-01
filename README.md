# 👋 Hi, I'm Esraa Kamel
## Senior Agentic AI Engineer | LLM Orchestration & Multi-Agent Systems Specialist

![Banner](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

### 🚀 About Me
I am a **Senior Agentic AI Engineer** specializing in the orchestration of autonomous, goal-oriented AI systems. My work focuses on moving beyond simple chat interfaces to building **production-grade agentic workflows** that possess reasoning, planning, and self-healing capabilities. I architect multi-agent systems that solve complex, non-linear problems at scale.

- 🔭 **Currently Architecting:** A distributed multi-agent swarm for automated software engineering.
- 🧠 **Core Expertise:** LLM Reasoning (CoT/ToT), Agentic RAG, Tool-Use Optimization, and Multi-Agent Orchestration.
- 🌱 **Deep Diving:** Exploring the intersection of **Small Language Models (SLMs)** and edge-based agentic reasoning.
- 👯 **Open Source:** Active contributor to **[aden-hive/hive](https://github.com/aden-hive/hive)** (Agentic Framework Internals).
- 💬 **Consulting:** Helping enterprises transition from "Chatbots" to "Agentic Workforces".

---

### 🏗️ Engineering Philosophy: Designing for Failure
I build production agentic AI systems where failure is handled, not hoped away. While most systems are designed for the "happy path," I design for the **rate limits at step 3**, the **approvals that arrive 4 hours later**, and the **platforms that redesign their UI overnight**.

#### My 6 Hard Constraints for Production Agents:
1. **Single Responsibility:** Every agent answers exactly one question to isolate failure modes.
2. **Deterministic Routing:** Routing is pure Python, not LLM-driven, for testability and version control.
3. **Mandatory Verification:** Post-action verification is a hard checkpoint before state advances.
4. **Durable HITL:** Human-in-the-loop is a named graph node that survives process restarts and deployments.
5. **Architectural Boundaries:** Action limits are compile-time constants, not prompt-level suggestions.
6. **Hybrid Retrieval:** Dense + sparse retrieval with cross-encoder re-ranking for real-world query variance.

---

### 🛠️ Signature Architectural Patterns
These patterns are the foundation of every production system I build, ensuring reliability, security, and resilience in non-deterministic environments.

| Pattern | Description | Justification |
| :--- | :--- | :--- |
| **PAV (Perception-Action-Verify)** | A vision-guided loop where a PerceptionAgent analyzes screenshots to guide actions and verify outcomes. | Eliminates reliance on brittle CSS selectors; ensures the agent "sees" the result of its work. |
| **UNVERIFIABLE State** | A first-class state for actions that executed correctly but cannot be confirmed due to propagation delays. | Prevents duplicate actions from retries and maintains system honesty during async processing. |
| **API-First with Browser Fallback** | Automatic transition to browser automation when API endpoints fail or are unavailable. | Ensures 100% task completion regardless of external API stability or coverage. |
| **Capability Self-Calibration** | Real-time reliability tracking that auto-disables/re-enables tools based on health checks. | Prevents cascading failures and optimizes routing toward the most stable execution path. |
| **Audit Hash Chains** | Append-only logs where each row contains a SHA-256 hash of itself and the previous row. | Provides tamper-evident proof of every agent action and decision for high-stakes environments. |

---

### 🛠️ Tech Stack

| Category | Tools & Technologies |
| :--- | :--- |
| **Agent Frameworks** | ![LangGraph](https://img.shields.io/badge/LangGraph-000000?style=flat-square&logo=graph&logoColor=white) ![CrewAI](https://img.shields.io/badge/CrewAI-FF4B4B?style=flat-square&logo=python&logoColor=white) ![PydanticAI](https://img.shields.io/badge/PydanticAI-E92063?style=flat-square&logo=pydantic&logoColor=white) ![Semantic Kernel](https://img.shields.io/badge/Semantic--Kernel-0078D4?style=flat-square&logo=microsoft&logoColor=white) |
| **LLMs & APIs** | ![GPT-4o](https://img.shields.io/badge/GPT--4o-412991?style=flat-square&logo=openai&logoColor=white) ![Claude 3.5](https://img.shields.io/badge/Claude--3.5-D97757?style=flat-square&logo=anthropic&logoColor=white) ![Llama 3](https://img.shields.io/badge/Llama--3-0467DF?style=flat-square&logo=meta&logoColor=white) ![Mistral](https://img.shields.io/badge/Mistral-FD6F00?style=flat-square&logo=mistral&logoColor=white) |
| **Vector DBs** | ![Pinecone](https://img.shields.io/badge/Pinecone-27272E?style=flat-square&logo=pinecone&logoColor=white) ![Weaviate](https://img.shields.io/badge/Weaviate-00D1FF?style=flat-square&logo=weaviate&logoColor=white) ![Milvus](https://img.shields.io/badge/Milvus-00BFFF?style=flat-square&logo=milvus&logoColor=white) ![Chroma](https://img.shields.io/badge/Chroma-FF6F61?style=flat-square&logo=googlecloud&logoColor=white) |
| **Backend & Infra** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) |
| **Monitoring & Eval** | ![LangSmith](https://img.shields.io/badge/LangSmith-000000?style=flat-square&logo=chainlink&logoColor=white) ![Weights & Biases](https://img.shields.io/badge/W%26B-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=white) ![Arize Phoenix](https://img.shields.io/badge/Arize-000000?style=flat-square&logo=arize&logoColor=white) |

---

### 🌟 Featured Projects

#### 🛡️ Security & Adversarial AI
- **AI Product Red-Team Agent:** LangGraph · AutoGen · Claude API · FastAPI · Redis. Lethal Trifecta injection · CVSS-scored vulnerability reports.
- **Automated Code Compliance & Security Agent:** AWS Bedrock · Guardrails · GitHub Webhooks · Terraform. 100% policy adherence · 60% reduction in code review time.
- **Agentic Supply Chain Orchestrator:** Azure AI Foundry · RAG · GPT-4o · 5 agents. BOM → PO with zero manual steps · 100% error detection.

#### 🤖 Autonomous QA & Testing
- **Autonomous QA Agent Framework:** LangGraph · ChromaDB · GitHub Actions · pytest · 8 agents. Full test lifecycle: PR diff → generation → self-healing → defect filing.
- **Self-Healing Selenium Framework:** LangGraph · Selenium · PostgreSQL · 6 agents. DOM-aware repair · confidence-gated HITL · autonomous commit on high confidence.
- **Agentic Defect Intelligence Pipeline:** LangGraph · Qdrant · Kafka · hybrid RAG · 6 agents. Closed-loop: production failures → pre-release test coverage feedback.
- **Multi-Agent User Simulation & Chaos Lab:** LangGraph · LangChain · FastAPI · 4-layer architecture. Persona generation · chaos injection · behavioral anomaly detection.

---

### 🧪 Open Source Contributions

#### **[aden-hive/hive](https://github.com/aden-hive/hive)**
*Python · Agentic Framework Internals*
- **Impact:** 9 core contributions across bugs and features.
- **Key PRs:** #5923, #5855, #5918, #5760, #5805, #6214, #6542, #6555, #6605.

---

### 🎓 Credentials
- 🎓 **MSc in AI, Agentic AI & LLM Engineering** — Woolf University (in progress)
- 🎓 **BSc Computer Science** — Menoufia University
- ☁️ **AWS AI/ML Scholar 2025**

---

### 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=EsraaKamel11&show_icons=true&theme=tokyonight" height="170" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=EsraaKamel11&layout=compact&theme=tokyonight" height="170" />
</p>

---

### 📫 Connect with Me
<p align="left">
  <a href="https://www.linkedin.com/in/esraa-kamel0811/" target="blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:Israa.kamel811@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail" />
  </a>
</p>

---

### 💡 Quote of the Day
> "The best way to predict the future is to build an agent that creates it." — *AI Proverb*

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=EsraaKamel11&color=blue" alt="Visitor Count" />
</p>
