# Hoi, I'm Julius

### M.Sc. Artificial Intelligence @ UZH | Data Engineer @ Swissgrid

I'm an AI Master's student at the **University of Zurich**, with a background in **Statistics and Data Science** from **LMU Munich**. I build data platforms for energy and blockchain research, and study how to evaluate agents against exact, executable mechanisms. My interests connect data engineering, distributed systems, adversarial machine learning and verifiable agent evaluation.

---

### 🚀 Currently...

- **Data Engineer at Swissgrid** (Performance Monitoring), building energy-market ETL pipelines, an ENTSO-E transformation microservice, and the validation, orchestration and monitoring around them.
- **Building MAP** at UZH: a self-hosted blockchain research platform, with current work on reliable history APIs and a Kubernetes/GitOps migration.
- **Developing ChainKernel**, my Master's thesis project on execution-verified tasks for agents interacting with deployed programs.


---

### 🛠 Tech Stack

| Category | Tools & Technologies |
| :--- | :--- |
| **Languages** | Python, SQL, C++, Java |
| **Data & Storage** | ClickHouse, Kafka, Redis, Elasticsearch, Delta Lake (shadow pipeline) |
| **Pipelines & Orchestration** | Temporal, Camunda, FME, Spark Structured Streaming |
| **Platform & DevOps** | Docker, Kubernetes (kind rehearsals; k3s migration in progress), Kustomize, Argo CD, GitHub Actions, GHCR, Git |
| **Services** | FastAPI, REST API design, scoped access control, distributed rate limiting, XSD/XML validation |
| **Observability** | Prometheus, Grafana, OpenTelemetry, Grafana Tempo, Tableau, Weights & Biases |
| **AI / ML** | PyTorch, reinforcement learning, multi-agent learning, NLP/RAG, LSTMs/GRUs |
| **Verification** | Foundry, differential testing, exact integer simulation, historical replay |

---

### 🧪 Featured Projects

#### 🧱 MAP — Multichain Analytics Platform

*University of Zurich, Blockchain & DLT Group — Master's Project & Independent Study*

- **Ethereum data at scale:** a stored release covering **26M+ blocks**, a **3.73B-event token-transfer index**, and a discovery catalog of **1.83M contracts** in ClickHouse.
- **Durable ingestion:** Cryo/web3.py → transactional Kafka → ClickHouse, orchestrated with **Temporal**, with **250-block checkpoints**, coverage tracking, restart-safe backfills and synchronization against the provider's finalized head.
- **Research access:** FastAPI APIs, scoped keys, normal/admin roles, Redis-backed request limits and project-table workspaces. Resumable Parquet imports include schema review and reconciliation; a **973 MB / 999,424-row** local trial completed alongside reads and chain ingestion.
- **Multichain validation:** bounded Alchemy pilots on **Polygon, Arbitrum, Base and BNB Smart Chain**, reconciling blocks, transactions and logs against frozen provider payloads over four blocks per chain.
- **Lakehouse prototype:** a blocks-only **Spark/Delta Lake shadow pipeline** with Bronze/Silver/Gold transformations, schema contracts and quarantine; replay, recovery and time travel tested on synthetic workloads up to **100K blocks**.
- **Current work:** snapshot-bound history pagination in an isolated, tested API release candidate, plus a **k3s/Argo CD** migration design for **dev → staging → production**. The serving platform currently runs on Docker Compose.

#### 🧠 DeFiTrials — Verifiable Tasks for Agents on Deployed Programs

*University of Zurich, Blockchain & DLT Group — Master's thesis project, in development*

- Designing three task families on pinned Ethereum state: **Predict** transaction effects, **Formalise** exact models from source or bytecode, and **Construct** transactions that reach a goal.
- Designing independent graders around **deterministic EVM re-execution**, hidden differential tests, symbolic equivalence and bounded infeasibility proofs, including unreachable goals that test whether an agent correctly declines.
- Building on an **exact integer Uniswap v3 engine** validated in **668 Foundry differential scenarios**. Planned evaluation includes frozen tool-using agents, counterfactual tasks to resist answer lookup, and a bounded **GRPO reward-signal study**.

#### 🔬 OracleBench — Adversarial Stress Testing for DeFi Price Oracles

- A configurable research framework for oracle manipulation, with exact Uniswap v3 mechanics, oracle and market parameters, and a Uniswap v4 truncated-oracle hook model.
- Historical replay validated on **90 held-out mainnet windows**, covering **7,336 trace-backed swaps**, with exact no-attack controls.
- Research directions include **reinforcement learning, self-play and PSRO** for discovering manipulation strategies and comparing mechanism robustness.

---

### 📫 Connect with me

- **LinkedIn:** [Julius Landes](https://linkedin.com/in/juliuslandes)
- **Languages:** German (Native), English (C1)

*Updated November 2026.*
