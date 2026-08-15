# Vishnu Pulipaka

AI & ML Engineer · Data Engineer · LLM Research · Dayton, Ohio, USA

[Email](mailto:vishnupulipaka22@gmail.com) · [GitHub](https://github.com/vishnup22) · [LinkedIn](https://linkedin.com/in/vishnup22) · [Hugging Face](https://huggingface.co/pulipakav-1)

I build production-grade intelligent systems end-to-end — multi-agent LLM platforms, RAG evaluation pipelines, distributed CDC architectures, GPU inference engines, and full-stack applications — and research low-resource language modeling and LLM fairness on the side. Currently open to **AI/ML Engineer** and **Data Engineer** roles.

---

## Projects

**AI Engineering**

- **[production-rag-eval-platform](https://github.com/vishnup22/production-rag-eval-platform)** — RAG evaluation platform benchmarking 3 retrievers against 3 LLM providers; 92% faithfulness and 100% retrieval hit rate, with GitHub Actions gates blocking prompt/retrieval regressions.
- **[FinSight-AI](https://github.com/vishnup22/FinSight-AI)** — 4-agent async financial research system across US, NSE, and BSE markets, combining FinBERT sentiment, LLM-as-judge scoring, and Markowitz portfolio optimization.
- **[Vocalytics](https://github.com/vishnup22/Vocalytics)** — Voice-to-SQL BI copilot over 3.4M orders / 30M+ line items; guarded SQL generation with dynamic allowlists and a 29-test eval suite.
- **[tok-adapt](https://github.com/vishnup22/tok-adapt)** — Python/CLI library for tokenizer and embedding-layer adaptation, plus an end-to-end CPT → SFT → DPO pipeline for cross-lingual LLM fine-tuning.

**Data Engineering**

- **[cdc-pipeline](https://github.com/vishnup22/cdc-pipeline)** — Exactly-once CDC pipeline sustaining 50,000 writes/min: PostgreSQL WAL → Debezium → Kafka → Flink → Apache Iceberg, chaos-tested against TaskManager kills and network partitions.
- **[data-lakehouse](https://github.com/vishnup22/data-lakehouse)** — Delta Lake compaction engine cutting per-partition file count 95% (87 → 4 files) in 14.5s with zero reader downtime.
- **[data-quality-ai](https://github.com/vishnup22/data-quality-ai)** — Real-time data quality and LLM incident-triage platform detecting 6 failure modes; HIGH-severity incidents flagged in under 42ms.

**ML Engineering**

- **[tensorrt-vision-server](https://github.com/vishnup22/tensorrt-vision-server)** — ResNet-50 compiled to an FP16 TensorRT 11 engine on CUDA 12.4; 3.55× throughput (97 → 347 FPS), 4.3× P99 latency cut, zero accuracy loss.
- **[feature-store-skew](https://github.com/vishnup22/feature-store-skew)** — Feast/PySpark/Redis feature store enforcing train-serve parity, with SHA-256 hash comparison catching skew at inference time.
- **[churn-ml](https://github.com/vishnup22/churn-ml)** — XGBoost churn pipeline with 50-trial Optuna tuning, an MLflow Registry promotion gate, and Evidently drift monitoring.

**Full-Stack**

- **[flowforge-automation-engine](https://github.com/vishnup22/flowforge-automation-engine)** — Visual workflow automation platform: React Flow editor, Spring Boot DAG executor, JWT auth, and OAuth credentials encrypted at rest (Jasypt AES-256).
- **[flash-sale-reservation-platform](https://github.com/vishnup22/flash-sale-reservation-platform)** — High-throughput flash-sale reservations with Redisson Redlock inventory holds, Kafka-backed checkout, and live seat availability over WebSocket.
- **[quire-workspace](https://github.com/vishnup22/quire-workspace)** — Real-time collaborative document editor with live multi-cursor editing via Yjs CRDTs, on a Spring Boot WebSocket hub.

## Research

Independent research in low-resource language modeling and LLM fairness, alongside my engineering work.

- **How Fast Can Reward Models Score?** — a systems study of C++ and PyTorch inference runtimes for RLHF reward scoring, finding the CPU speedup traces to ONNX Runtime's graph execution rather than C++ itself. [arXiv:2607.19712](https://arxiv.org/abs/2607.19712) · [code](https://github.com/vishnup22/reward-model-benchmarks)
- **Evaluating Dedicated Monolingual and Joint Multilingual Causal Models for Dravidian Languages** — 5 GPT-2-architecture models for Telugu, Tamil, Kannada, and Malayalam, benchmarked against XLM-R, mBERT, and mGPT on tokenizer efficiency and downstream transfer. [arXiv:2608.07727](https://arxiv.org/abs/2608.07727) · [code](https://github.com/vishnup22/dravidian-lm-research)
- **Release-Level Fairness Drift in Large Language Models** — a fairness-regression audit pipeline across 12 model versions from 5 providers, 6 model families, and 7 bias benchmarks (~200K examples). Under double-blind review. [code](https://github.com/vishnup22/fairness-drift-llms)

## Tech Stack

**AI/ML** — Python, PyTorch, TensorRT, CUDA, ONNX, Hugging Face Transformers, scikit-learn, XGBoost, Optuna
**LLM/NLP** — Claude, OpenAI, Ollama, ChromaDB, Sentence Transformers, SentencePiece, Whisper, FinBERT
**Data Engineering** — Kafka, Spark, Flink, Delta Lake, Iceberg, Debezium, PostgreSQL, Redis, DuckDB
**Full-Stack** — Java, Spring Boot, React, TypeScript, Yjs, WebSocket, JWT
**MLOps/Infra** — MLflow, FastAPI, Docker, GitHub Actions, Feast, Evidently, Prometheus

---

Open to collaborations, open-source contributions, and mentorship in AI/ML, data engineering, and NLP research — [reach out on LinkedIn](https://linkedin.com/in/vishnup22) or [email me](mailto:vishnupulipaka22@gmail.com).
