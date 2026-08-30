# Hoi, I'm Julius

### M.Sc. Artificial Intelligence @ UZH | Data Engineer @ Swissgrid

I'm an AI Master's student at the **University of Zurich**, with a background in **Statistics and Data Science** from **LMU Munich**. My work sits at the intersection of production data platform engineering and multi-agent machine learning — building pipelines that have to survive contact with real operational load, and studying systems where several strategic actors interact.

---

### 🚀 Currently...

* **Data Engineer at Swissgrid** (Performance Monitoring), building ETL pipelines, an ENTSO-E transformation microservice, and the monitoring and orchestration around them.
* **Building MAP**, a self-hosted, production-grade blockchain data platform at the UZH Blockchain Center — currently extending it toward Kubernetes, GitOps and a Delta Lake medallion architecture.
* **Finishing my Master's thesis** on identity-aware multi-agent representations for DeFi oracle security.

---

### 🛠 Tech Stack

| Category | Tools & Technologies |
| :--- | :--- |
| **Languages** | Python, SQL, C++, Java |
| **Data & Storage** | ClickHouse, Kafka, Delta Lake *(in progress)*, Elasticsearch, Redis |
| **Pipelines & Orchestration** | Temporal, Camunda, FME, Spark Structured Streaming *(in progress)* |
| **Platform & DevOps** | Docker, Kubernetes *(in progress)*, Helm, Argo CD, Terraform *(in progress)*, Git, CI/CD |
| **Services** | FastAPI, REST API design, multi-tenant auth & rate limiting, XSD/XML validation |
| **Observability** | Prometheus, Grafana, OpenTelemetry, Tableau, Weights & Biases |
| **AI / ML** | PyTorch, Multi-Agent RL, Self-Play (PSRO, FSP), CMDPs, NLP (RAG), LSTMs/GRUs |

---

### 🧪 Featured Projects

#### 🧱 MAP — Self-Hosted ETL & Lakehouse Platform for EVM Blockchain Data
*University of Zurich, Blockchain Center — Master's Project*

* Production-grade ETL ingesting seven canonical EVM data types (blocks, transactions, events, traces, contracts, native and ERC-20 transfers) across **25M+ Ethereum blocks** into **ClickHouse**, running as **22 Docker services** against a private Erigon archive node.
* **Kafka-buffered, Temporal-orchestrated** architecture that decouples the control plane from the data write path, enabling idempotent, restart-safe backfills of billions of rows.
* **Multi-tenant serving layer**: FastAPI REST API (16 workers), API-key auth with permission tiers, Redis-backed distributed rate limiting, atomically provisioned per-consumer ClickHouse workspaces.
* Protocol-decoding subsystem for curated protocols (Uniswap V2, Aave V3, ERC-20) and arbitrary user-registered contracts, including runtime discovery of dynamically created contracts.
* Full observability with **Prometheus + Grafana**; data integrity cross-validated against Dune Analytics and Etherscan to bit-identical aggregate results.
* **Now extending it:** Kubernetes with Helm and Argo CD (GitOps), object storage plus Delta Lake in a Bronze/Silver/Gold medallion design, Spark Structured Streaming, and explicit data contracts, quality gates, lineage and catalog metadata.

#### 🔮 Identity-Aware Multi-Agent Representations for DeFi Oracle Security
*Master's Thesis, University of Zurich*

* Models competitive price-oracle manipulation as a **finite-population multi-agent stochastic game**, where attackers jointly move the market price while competing individually for block inclusion and a downstream prize.
* Proves an **aggregate non-identifiability result**: identical aggregate order flow and oracle trajectories can imply different private manipulation costs, lower-bounding the error of purely aggregate representations.
* Designs an **identity-aware representation** separating anonymous market-impact statistics from contest-specific signals (bid rank, inclusion status, execution position, flow ahead).
* Role-indexed **JPSRO / coarse-correlated-equilibrium** evaluation with per-role deviation certificates and held-out best responses, under a 20-seed confirmatory protocol with paired bootstrap CIs and SHA-256 experiment manifests.

#### 🤖 Federated Safe Policy-Model Iteration (F-SPMI)
*Reinforcement Learning Research, University of Zurich*

* Parallelized variant of the **SPMI** algorithm for Configurable MDPs, using centralized federated learning principles to accelerate learning while preserving safety guarantees.
* Benchmarked greedy local selection against **GP-driven (UCB) exploration**, quantifying the trade-off between sample efficiency, scalability and asymptotic performance.
* Flexible Python framework supporting both tabular and neural network policies.

#### 🎬 Multi-Modal Movie QA Agent

* Hybrid QA system combining **symbolic reasoning (SPARQL)** with **latent space inference (TransE)** over the Wikidata knowledge graph.
* End-to-end pipeline for entity disambiguation and vector-based similarity search.

#### 📈 Deep Learning for Stock Market Gaps
*Bachelor Thesis*

* Comparative analysis of **LSTMs vs. GRUs** for detecting market volatility, with a **Double Deep Q-Network** agent simulating trading strategies in backtesting environments.
* WandB hyperparameter sweeps across 1000+ US companies.

---

### 📫 Connect with me

* **LinkedIn:** [Julius Landes](https://linkedin.com/in/juliuslandes)
* **Languages:** German (Native), English (C1)
