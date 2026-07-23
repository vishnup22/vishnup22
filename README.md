<div align="center">

<h1>Vishnu Pulipaka</h1>

<p><strong>AI & ML Engineer &nbsp;·&nbsp; Data Engineer &nbsp;·&nbsp; LLM Research</strong></p>

<img src="https://readme-typing-svg.demolab.com?font=Inter&weight=500&size=17&duration=3000&pause=1000&color=2563EB&center=true&vCenter=true&width=620&lines=Building+intelligent+systems+at+scale;LLM+Agents+%7C+RAG+Pipelines+%7C+MLOps+Automation;Real-time+CDC+%7C+Data+Lakehouses+%7C+GPU+Inference;Low-Resource+%26+Fairness-Focused+LLM+Research" alt="Typing SVG" />

<br/>

<a href="mailto:vishnupulipaka22@gmail.com"><img src="https://img.shields.io/badge/Email-vishnupulipaka22@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white"/></a>
&nbsp;
<a href="https://github.com/vishnup22"><img src="https://img.shields.io/badge/GitHub-vishnup22-181717?style=flat-square&logo=github&logoColor=white"/></a>
&nbsp;
<a href="https://linkedin.com/in/vishnup22"><img src="https://img.shields.io/badge/LinkedIn-vishnup22-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
&nbsp;
<img src="https://img.shields.io/badge/%F0%9F%9F%A2%20Open%20to%20Work-Available%20Now-22c55e?style=flat-square"/>
&nbsp;
<img src="https://komarev.com/ghpvc/?username=vishnup22&color=6b7280&style=flat-square&label=Profile+Views"/>

</div>

---

### About

I build production-grade intelligent systems end-to-end — multi-agent LLM platforms, RAG evaluation pipelines, distributed CDC architectures, and GPU inference engines — and I research low-resource language modeling and LLM fairness on the side. Comfortable owning a system from data pipeline to model to deployment.

Currently seeking **AI/ML Engineer** or **Data Engineer** roles.

**Highlights:** 3.55× GPU inference throughput · 50K writes/min CDC pipeline with proven exactly-once delivery · 92% RAG faithfulness with CI/CD quality gates · fairness-drift study across 12 LLM releases (EMNLP 2026 submission)

---

## Engineering Projects

<div align="center">

<a href="https://github.com/vishnup22/cdc-pipeline"><img src="https://github-readme-stats.vercel.app/api/pin/?username=vishnup22&repo=cdc-pipeline&theme=default&hide_border=true&title_color=1e293b&text_color=374151" height="150"/></a>
<a href="https://github.com/vishnup22/production-rag-eval-platform"><img src="https://github-readme-stats.vercel.app/api/pin/?username=vishnup22&repo=production-rag-eval-platform&theme=default&hide_border=true&title_color=1e293b&text_color=374151" height="150"/></a>

<a href="https://github.com/vishnup22/tensorrt-vision-server"><img src="https://github-readme-stats.vercel.app/api/pin/?username=vishnup22&repo=tensorrt-vision-server&theme=default&hide_border=true&title_color=1e293b&text_color=374151" height="150"/></a>
<a href="https://github.com/vishnup22/data-lakehouse"><img src="https://github-readme-stats.vercel.app/api/pin/?username=vishnup22&repo=data-lakehouse&theme=default&hide_border=true&title_color=1e293b&text_color=374151" height="150"/></a>

<a href="https://github.com/vishnup22/FinSight-AI"><img src="https://github-readme-stats.vercel.app/api/pin/?username=vishnup22&repo=FinSight-AI&theme=default&hide_border=true&title_color=1e293b&text_color=374151" height="150"/></a>
<a href="https://github.com/vishnup22/Vocalytics"><img src="https://github-readme-stats.vercel.app/api/pin/?username=vishnup22&repo=Vocalytics&theme=default&hide_border=true&title_color=1e293b&text_color=374151" height="150"/></a>

</div>

### [Distributed CDC Pipeline — Exactly-Once Delivery](https://github.com/vishnup22/cdc-pipeline)
`PostgreSQL WAL → Debezium → Kafka → PyFlink → Apache Iceberg`

Sustains **50,000 writes/min** with mathematically proven exactly-once delivery via Flink checkpoint barriers, two-phase Iceberg atomic commits, and `(entity_id, LSN, operation_type)` idempotency keys.

<details>
<summary>Details & metrics</summary>
<br>

| | |
|---|---|
| Throughput | 50,000 writes/min |
| Checkpointing | RocksDB · **281ms** checkpoints |
| Resilience | Chaos-tested — survives TaskManager kills & network partitions, zero data loss |
| Validation | DuckDB post-recovery assertions confirm exactly-once semantics |

</details>

### [RAG Evaluation Platform with CI/CD Quality Gates](https://github.com/vishnup22/production-rag-eval-platform)
`ChromaDB · BM25 · OpenAI · Anthropic · Ollama`

3 retrievers, 3 LLM providers, 7 automated metrics over an 8-case golden QA suite — GitHub Actions blocks merges that regress retrieval or faithfulness.

<details>
<summary>Details & metrics</summary>
<br>

| Metric | Result |
|--------|--------|
| Faithfulness | **92%** |
| Retrieval hit rate | **100%** |
| Merge protection | GitHub Actions blocks regressions |

</details>

### [TensorRT Inference Optimization Engine](https://github.com/vishnup22/tensorrt-vision-server)
`TensorRT 11 · CUDA 12.4 · PyTorch · ONNX · C++ Crow`

ResNet-50 compiled to FP16 TensorRT 11 on CUDA 12.4 and served via a C++ HTTP server, with zero accuracy loss.

<details>
<summary>Details & metrics</summary>
<br>

| Metric | Before | After | Gain |
|--------|--------|-------|------|
| Throughput | 97 FPS | **347 FPS** | **3.55×** |
| P99 Latency | 21.4 ms | **4.9 ms** | **4.3×** |
| Accuracy (10K CIFAR-10) | 95.02% | 95.03% | ✅ Zero loss |

</details>

### [Tiered Data Lakehouse Compaction Engine](https://github.com/vishnup22/data-lakehouse)
`Kafka · Spark Structured Streaming · Delta Lake`

Python compaction daemon cutting per-partition file count by **95%** (87 → 4 files) in 14.5 seconds, with zero reader downtime.

<details>
<summary>Details & metrics</summary>
<br>

| | |
|---|---|
| Compaction | 87 → 4 files per partition in 14.5s |
| Consistency | Delta ACID `replaceWhere` + MVCC snapshot isolation |
| Testing | 77 pytest tests · DuckDB before/after benchmarks |

</details>

### [FinSight-AI — Multi-Agent Stock Analysis Platform](https://github.com/vishnup22/FinSight-AI)
`FastAPI · FinBERT · ChromaDB · asyncio`

4-agent financial research system (fundamental · technical · sentiment · risk) with async orchestration across US, NSE, and BSE markets.

<details>
<summary>Details & metrics</summary>
<br>

| | |
|---|---|
| Skills | `/analyse` `/compare` `/portfolio` `/backtest` `/sector` `/digest` |
| Quality gate | LLM-as-judge · 5 dimensions scored · **≥ 7 / 10 pass threshold** |
| RAG | ChromaDB + all-MiniLM-L6-v2 · FinBERT live news sentiment |
| Optimization | Markowitz max-Sharpe + equal-weight portfolio backtesting |

</details>

### [VocalLytics — Voice-to-SQL Analytics Platform](https://github.com/vishnup22/Vocalytics)
`Claude · Whisper · PostgreSQL · Plotly`

Voice-to-SQL BI copilot processing Instacart-scale data (~3.4M orders, **30M+ line items**). Converts natural-language voice queries into guarded SQL and interactive charts.

<details>
<summary>Details & metrics</summary>
<br>

| | |
|---|---|
| Data scale | ~3.4M orders · 30M+ line items |
| Upload support | CSV ≤ 8 MB · schema inference up to 60 columns × 5,000 rows |
| Security | Dynamic SQL allowlists · guarded query generation |
| Quality | NL-to-SQL eval suite · **29 passing tests** |

</details>

<details>
<summary><strong>More engineering projects</strong> — Telco Churn MLOps · Feature Store Skew Detection · Data Quality & Incident Triage</summary>

### [Telco Churn Prediction — MLOps Pipeline](https://github.com/vishnup22/churn-ml)
`XGBoost · MLflow · Evidently · GitHub Actions`

XGBoost churn classifier on 7,043 records / 21 features with a full automated MLOps lifecycle: 50-trial Optuna HPO, 5-fold stratified CV, PR-AUC **0.65** / Recall **≥ 0.70**, and a champion-promotion gate in the MLflow Registry (≤ 0.01 PR-AUC regression tolerance). Weekly batch scoring + retraining via GitHub Actions, drift monitored with Evidently.

### [ML Feature Store & Train-Serve Skew Detection](https://github.com/vishnup22/feature-store-skew)
`PySpark · Feast · Redis · FastAPI`

End-to-end feature pipeline on NYC Taxi data enforcing strict train-serve parity. Features computed once in PySpark → Feast offline store (training) → Redis (inference); skew caught at serving time via SHA-256 feature matrix hashes and column-order validation, backed by a 9-test pytest suite.

### [AI-Powered Data Quality & Incident Triage Platform](https://github.com/vishnup22/data-quality-ai)
`Kafka · PostgreSQL · FastAPI · Prometheus`

Real-time data quality platform detecting 6 failure modes (nulls, negatives, schema drift, malformed timestamps, duplicates, unsupported versions). HIGH-severity incidents generated in **< 42ms**, 12% dirty-batch quarantine rate, LLM triage producing root-cause JSON with severity scoring and remediation steps (mock / Ollama / OpenAI backends), 10 FastAPI endpoints, Prometheus scrape endpoint.

</details>

---

## Research

Independent research in low-resource language modeling and LLM fairness, alongside my engineering work.

<div align="center">

<a href="https://github.com/vishnup22/fairness-drift-llms"><img src="https://github-readme-stats.vercel.app/api/pin/?username=vishnup22&repo=fairness-drift-llms&theme=default&hide_border=true&title_color=1e293b&text_color=374151" height="150"/></a>
<a href="https://github.com/vishnup22/dravidian-lm-research"><img src="https://github-readme-stats.vercel.app/api/pin/?username=vishnup22&repo=dravidian-lm-research&theme=default&hide_border=true&title_color=1e293b&text_color=374151" height="150"/></a>

<a href="https://github.com/vishnup22/BabyLM"><img src="https://github-readme-stats.vercel.app/api/pin/?username=vishnup22&repo=BabyLM&theme=default&hide_border=true&title_color=1e293b&text_color=374151" height="150"/></a>
<a href="https://github.com/vishnup22/reward-model-benchmarks"><img src="https://github-readme-stats.vercel.app/api/pin/?username=vishnup22&repo=reward-model-benchmarks&theme=default&hide_border=true&title_color=1e293b&text_color=374151" height="150"/></a>

</div>

### [Release-Level Fairness Drift in Large Language Models](https://github.com/vishnup22/fairness-drift-llms)
`EMNLP 2026 submission`

Fairness-regression audit pipeline measuring whether newer LLM releases are fairer, less fair, or differently biased than their predecessors — not just whether a single model is biased.

<details>
<summary>Details & findings</summary>
<br>

- Evaluated fairness drift across **12 model versions** from 5 providers and 6 model families, using 7 public bias benchmarks and ~200K prompt-response pairs
- Defines drift as D_f(M_t, M_t+1) = f(M_t+1) − f(M_t) across sentiment, toxicity, and stereotype metrics
- Toxicity declines slightly on average across newer releases, but individual transitions are non-monotonic
- Stereotype proxy scores stay flat or increase in most release transitions; Gemini 2.5 Pro shows a statistically significant stereotype increase
- Sentiment, toxicity, and stereotype scores are weakly correlated (`|r| < 0.2`) — fairness is multidimensional, and safety improvements don't guarantee representational-fairness improvements

</details>

### [Dravidian LM Research](https://github.com/vishnup22/dravidian-lm-research)
`GPT-2 · SentencePiece · HuggingFace Transformers`

Reproducible pretraining and benchmarking pipeline for Dravidian language models, built as a research artifact rather than a one-off training folder.

<details>
<summary>Details & scope</summary>
<br>

- Monolingual language modeling for **Telugu, Kannada, Tamil, and Malayalam**
- Corpus collection from CC100, Wikipedia, Samanantar, and TinyStories
- SentencePiece tokenizer training + GPT-2 pretraining as the first implemented architecture
- Config-driven experiment execution with cross-language/cross-run result logging
- Planned: additional architectures beyond GPT-2, broader evaluation and benchmarking

</details>

### [BabyLM 2026 Challenge — Baselines & Data Translation](https://github.com/vishnup22/BabyLM)
`GPT-2 · IndicTrans2 · Multilingual NLP`

Baselines for the 2026 BabyLM Challenge (Strict / Strict-Small / Multilingual tracks), plus a companion pipeline ([`babylm_data_translation`](https://github.com/vishnup22/babylm_data_translation)) translating the BabyLM Strict corpus from English into Hindi and Telugu.

<details>
<summary>Details & scope</summary>
<br>

- GPT-2 baseline (`strict-gpt2`) and last year's interaction-track baseline adapted to Strict/Strict-Small (`strict-interaction`)
- Translation via IndicTrans2 (`ai4bharat/indictrans2-en-indic-1B`, 1B-parameter open NMT model) across all 6 BabyLM sub-corpora (BNC Spoken, CHILDES, Gutenberg, OpenSubtitles, Simple Wiki, Switchboard)
- Produces sentence-level parallel Hindi/Telugu/English corpora for train, dev, and test splits

</details>

### [RLHFast — Reward Model Inference Benchmarks](https://github.com/vishnup22/reward-model-benchmarks)
`C++ · ONNX Runtime · PyTorch · torch.compile`

Systems benchmark asking a narrow empirical question: how much does a native C++ inference engine actually buy you over standard Python serving paths for RLHF reward-model scoring, and where does that speed come from?

<details>
<summary>Details & findings</summary>
<br>

- Native C++ engine beats every Python baseline on CPU with no overlap in confidence intervals; on GPU it beats HF eager mode and FastAPI, though `torch.compile` edges it out at the median
- **The advantage comes from ONNX Runtime, not from C++** — calling the same ONNX session from Python costs the same as from C++ within noise
- Naive batching hurts throughput on every system tested; length-aware batch scheduling recovers it, but only on GPU
- Native (non-Python) tokenization is the only named C++ optimization with a measurable effect (~3.8× faster tokenization)
- Core finding reproduces — and is larger — on a second architecture (Electra, WordPiece tokenizer)

</details>

---

## Tech Stack

**AI & Machine Learning**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![TensorRT](https://img.shields.io/badge/TensorRT-76B900?style=flat-square&logo=nvidia&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA_12.4-76B900?style=flat-square&logo=nvidia&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=flat-square&logo=onnx&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-189ABF?style=flat-square)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Optuna](https://img.shields.io/badge/Optuna-3B4EFF?style=flat-square)

**LLMs, RAG & NLP Research**

![Anthropic](https://img.shields.io/badge/Claude-191919?style=flat-square&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square)
![FinBERT](https://img.shields.io/badge/FinBERT-Sentiment-0A66C2?style=flat-square)
![ChromaDB](https://img.shields.io/badge/ChromaDB-Vector_DB-2563EB?style=flat-square)
![Sentence Transformers](https://img.shields.io/badge/Sentence_Transformers-6b7280?style=flat-square)
![SentencePiece](https://img.shields.io/badge/SentencePiece-Tokenization-6b7280?style=flat-square)
![Whisper](https://img.shields.io/badge/Whisper-412991?style=flat-square&logo=openai&logoColor=white)

**Data Engineering**

![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apache-kafka&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Apache Flink](https://img.shields.io/badge/Apache_Flink-E6526F?style=flat-square&logo=apacheflink&logoColor=white)
![Debezium](https://img.shields.io/badge/Debezium_CDC-E52828?style=flat-square)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-003366?style=flat-square)
![Apache Iceberg](https://img.shields.io/badge/Apache_Iceberg-1A73E8?style=flat-square)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logoColor=black)
![MinIO / S3](https://img.shields.io/badge/MinIO%20%2F%20S3-C72E49?style=flat-square&logo=amazons3&logoColor=white)

**MLOps & Infrastructure**

![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![Feast](https://img.shields.io/badge/Feast-FF6B35?style=flat-square)
![Evidently](https://img.shields.io/badge/Evidently_AI-9C27B0?style=flat-square)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

---

## GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=vishnup22&show_icons=true&theme=default&hide_border=true&include_all_commits=true&count_private=true&title_color=1e293b&icon_color=2563EB&text_color=374151" height="165"/>
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=vishnup22&layout=compact&theme=default&hide_border=true&langs_count=7&title_color=1e293b&text_color=374151" height="165"/>
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=vishnup22&theme=default&hide_border=true&date_format=M%20j%5B%2C%20Y%5D&ring=2563EB&fire=2563EB&currStreakLabel=2563EB" width="65%"/>
</div>

---

## Let's Connect

I'm actively looking for **AI/ML Engineer** or **Data Engineer** roles, and always open to **collaborations**, **open source contributions**, and **mentorship** in AI/ML, data engineering, and NLP research.

<div align="center">

<a href="https://linkedin.com/in/vishnup22"><img src="https://img.shields.io/badge/Message_on_LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
&nbsp;
<a href="mailto:vishnupulipaka22@gmail.com"><img src="https://img.shields.io/badge/Send_an_Email-EA4335?style=flat-square&logo=gmail&logoColor=white"/></a>

</div>

---

<div align="center">
<sub>Last updated · July 2026</sub>
</div>
