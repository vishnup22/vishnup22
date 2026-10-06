# Vishnu Pulipaka

### AI Engineer · LLM Systems · AI Research

I work on **LLM systems, model evaluation, multilingual NLP, inference, AI agents, memory, and increasingly Physical AI and Robotics**.

My work is centered on building AI systems that can be **measured, stress-tested, adapted, and improved systematically**.

On the engineering side, I build retrieval systems, agentic pipelines, inference infrastructure, evaluation frameworks, and model adaptation workflows.

On the research side, I study **low-resource language modeling, retrieval reliability, fairness drift, efficient inference, memory in intelligent systems, and how AI systems can move from purely digital reasoning toward interaction with the physical world**.

I am especially interested in the intersection of:

**LLMs × Memory × Agents × Robotics × Physical AI**

[GitHub](https://github.com/vishnup22) · [Hugging Face](https://huggingface.co/pulipakav-1) · [LinkedIn](https://linkedin.com/in/vishnup22) · [Email](mailto:vishnupulipaka22@gmail.com)

---

## What I Am Working Toward

I am interested in AI systems that do more than generate text.

The direction I care about most is building systems that can:

- reason over long horizons
- retrieve and preserve useful information
- maintain persistent memory
- learn from interaction
- coordinate multiple agents
- adapt models to new domains and languages
- operate efficiently under real system constraints
- connect perception, reasoning, memory, and action
- eventually interact reliably with the physical world

That naturally pulls my work toward:

**LLM Systems**  
**Agentic AI**  
**AI Memory**  
**Retrieval & Evaluation**  
**Multilingual NLP**  
**Post-Training**  
**Efficient Inference**  
**Physical AI**  
**Robotics**

A question that appears across much of my work is:

> **How do we know an intelligent system actually became better, rather than simply more complex?**

That means evaluation is usually part of the architecture from the beginning.

---

# Selected AI Engineering

## Production RAG Evaluation Platform

[GitHub](https://github.com/vishnup22/production-rag-eval-platform)

A RAG experimentation and regression-testing platform for measuring changes across both the retrieval and generation layers.

The system benchmarks:

- 3 retrieval configurations
- 3 LLM providers
- retrieval hit rate
- faithfulness
- answer quality
- latency
- regression behavior

Current evaluation results include:

**100% retrieval hit rate**  
**92% faithfulness**

The main goal is not simply achieving a strong benchmark.

The evaluation layer is integrated with **GitHub Actions**, allowing changes to prompts, retrieval strategies, or generation behavior to fail automated quality gates before they reach production.

The broader idea is to treat RAG quality as a **regression-testing problem**.

---

## FinSight AI

[GitHub](https://github.com/vishnup22/FinSight-AI)

A multi-agent financial research system built around four asynchronous agents operating across **US, NSE, and BSE markets**.

The pipeline combines:

**agent orchestration → retrieval → financial sentiment → structured reasoning → LLM evaluation → portfolio optimization**

Core components include:

- asynchronous agent coordination
- FinBERT sentiment analysis
- structured research outputs
- LLM-as-judge evaluation
- Markowitz portfolio optimization

My interest here is less about creating multiple agents and more about the deeper systems problems:

- task decomposition
- agent handoffs
- context management
- evaluation
- failure propagation
- state and memory
- reliability over multi-step workflows

---

## tok-adapt

[GitHub](https://github.com/vishnup22/tok-adapt)

A Python library and CLI for adapting pretrained language models to new languages and domains.

The project supports:

- tokenizer expansion
- vocabulary replacement
- embedding adaptation
- weight initialization
- continued pretraining
- supervised fine-tuning
- DPO

The repository includes an end-to-end:

**CPT → SFT → DPO**

pipeline for cross-lingual model adaptation.

The project grew from an interest in an often overlooked part of multilingual modeling: **the interface between tokenization, representation capacity, and downstream learning**.

---

## TensorRT Vision Inference Server

[GitHub](https://github.com/vishnup22/tensorrt-vision-server)

An inference systems project studying the impact of TensorRT compilation on ResNet-50 serving performance.

A ResNet-50 model was compiled to an **FP16 TensorRT 11 engine on CUDA 12.4**.

Measured results:

**97 FPS → 347 FPS**

with:

- **3.55× higher throughput**
- **4.3× lower P99 latency**
- **zero measured accuracy loss**

The project focuses on reproducible performance measurement rather than treating inference optimization as a black box.

---

## Vocalytics

[GitHub](https://github.com/vishnup22/Vocalytics)

A voice-driven analytical copilot operating over:

**3.4M orders**  
**30M+ line items**

The system converts spoken or natural-language questions into analytical SQL while restricting what the model is allowed to execute.

The execution layer includes:

- dynamic allowlists
- schema validation
- guarded SQL generation
- query restrictions
- evaluation against a 29-test suite

The interesting systems problem here is the boundary between:

**probabilistic model output**  
and  
**deterministic execution**

---

# Research

My research focuses on **language models, evaluation, inference, multilingual NLP, reliability, and emerging intelligent-system architectures**.

I am particularly interested in work where research questions can be tested through real systems rather than isolated model demos.

---

## Evaluating Dedicated Monolingual and Joint Multilingual Causal Models for Dravidian Languages

[arXiv](https://arxiv.org/abs/2608.07727) · [Code](https://github.com/vishnup22/dravidian-lm-research)

A study of causal language modeling across:

**Telugu · Tamil · Kannada · Malayalam**

I trained and evaluated dedicated language models and compared them with multilingual baselines.

Evaluation includes:

- language-model loss
- perplexity
- bits per byte
- tokenizer efficiency
- sentiment classification
- named-entity recognition

The broader research question is whether multilingual transfer outweighs the benefits of **language-specific tokenization and model capacity** under constrained data and compute.

---

## How Fast Can Reward Models Score?

[arXiv](https://arxiv.org/abs/2607.19712) · [Code](https://github.com/vishnup22/reward-model-benchmarks)

A systems study of reward-model inference for RLHF pipelines.

The work compares PyTorch and ONNX Runtime execution paths and investigates where CPU inference speedups actually originate.

The main finding is that the performance advantage is driven primarily by **ONNX Runtime execution and graph optimization**, rather than simply by moving inference into C++.

The work sits at the intersection of:

**RLHF infrastructure · inference systems · benchmarking · systems analysis**

---

## Release-Level Fairness Drift in Large Language Models

[Code](https://github.com/vishnup22/fairness-drift-llms)

A longitudinal study of whether fairness behavior remains stable when model providers release new versions.

The evaluation spans:

**12 model versions**  
**5 providers**  
**6 model families**  
**7 bias benchmarks**  
**~200K evaluation examples**

The central idea is to treat fairness as a **continuous regression-testing problem** rather than a one-time benchmark.

A newer model can improve overall while still regressing on specific behavioral dimensions.

**Status:** under double-blind review.

---

## Retrieval Stability Research

I am also working on methods for **certifying top-k retrieval stability under multi-agent communication**.

The work studies when a retrieval ranking can be guaranteed to remain unchanged under bounded perturbations introduced through agent communication.

Experiments include:

- HotpotQA
- 2WikiMultihopQA
- MuSiQue
- dense retrieval
- predictive certificates
- pairwise stability certificates

The goal is to move from simply observing retrieval changes toward reasoning about **when retrieval is provably stable**.

---

# Memory Research

One area I am increasingly interested in is **memory for intelligent systems**.

Current LLM applications are often powerful within a single context window but much weaker at maintaining coherent knowledge and behavior across long-running interactions.

I am interested in questions such as:

- what information should an agent remember?
- what should it forget?
- how should memories be retrieved?
- how should memories be consolidated over time?
- when should stored memory override or complement retrieval?
- how should memory reliability be evaluated?
- how do we prevent stale or incorrect memories from propagating?
- how should multiple agents share or isolate memory?
- can an AI system build abstractions from repeated experiences rather than simply storing transcripts?

I am particularly interested in architectures combining:

**episodic memory**  
**semantic memory**  
**retrieval systems**  
**working memory**  
**long-term agent state**  
**memory consolidation**

My long-term interest is in AI systems that do not simply respond to context, but **accumulate useful experience over time**.

---

# Physical AI & Robotics

I am increasingly interested in **Physical AI** — systems where perception, reasoning, memory, planning, and action interact with the real world.

Large models are rapidly becoming capable reasoning components, but physical environments introduce a very different set of constraints:

- partial observability
- real-time decision making
- sensor noise
- uncertainty
- safety constraints
- long-horizon planning
- embodiment
- continual interaction

I am interested in the connection between:

**vision-language models**  
**vision-language-action models**  
**robot learning**  
**world models**  
**multimodal reasoning**  
**planning**  
**memory**  
**reinforcement learning**  
**embodied agents**

The direction that interests me most is combining:

> **Perception + Reasoning + Memory + Action**

into systems that can learn from previous interactions and become more capable over time.

I am especially interested in exploring how LLM and agent research can transfer into robotics, including:

- robotic planning
- embodied agents
- manipulation
- multimodal foundation models
- robot memory
- human-robot interaction
- autonomous task execution
- simulation-to-real learning
- long-horizon robot reasoning

---

# How I Think About AI Systems

Most of the AI systems I build can be viewed through four layers.

### Model

Training, adaptation, inference, retrieval, multimodal perception, or agent reasoning.

### Memory

What information persists, how it is represented, when it is retrieved, and how it changes over time.

### Evaluation

Metrics, benchmarks, regression testing, failure analysis, and ablations.

### Systems

Latency, throughput, reproducibility, observability, reliability, and deployment behavior.

The work I enjoy most is:

> **building the system, measuring the system, breaking the system, understanding why it failed, and rebuilding it better.**

---

# Technical Focus

### Language Models

PyTorch · Hugging Face Transformers · Sentence Transformers · SentencePiece · FinBERT · Whisper

### LLM Systems

RAG · Agents · LLM Evaluation · LLM-as-Judge · Retrieval · Structured Generation · Prompt Regression Testing

### Training & Adaptation

Continued Pretraining · Supervised Fine-Tuning · DPO · Tokenizer Adaptation · Embedding Adaptation

### Inference

CUDA · TensorRT · ONNX Runtime · Quantization · Batching · Latency Benchmarking

### AI Systems

FastAPI · MLflow · Docker · GitHub Actions · Prometheus · Evidently

### Research

Experimental Design · Ablation Studies · Benchmark Construction · Statistical Evaluation · Multilingual NLP

### Areas I Am Expanding Into

Physical AI · Robotics · Vision-Language Models · Vision-Language-Action Models · Robot Learning · World Models · Reinforcement Learning · Embodied AI

---

# Research Interests

My current research interests include:

- LLM evaluation
- multilingual NLP
- low-resource language modeling
- AI agents
- agent evaluation
- AI memory
- long-term memory architectures
- retrieval reliability
- post-training
- efficient inference
- fairness and model behavior
- multimodal foundation models
- Physical AI
- robotics
- embodied intelligence
- robot learning
- world models

---

# Direction

I am most interested in building AI systems that can:

**reason**  
**remember**  
**retrieve**  
**adapt**  
**learn from interaction**  
**operate efficiently**  
**act in the physical world**

The long-term direction I find most compelling is intelligent systems that combine:

> **Models + Memory + Agents + Perception + Action**

rather than treating each of those as separate research problems.

---

## Open To

**AI Engineer**  
**ML Engineer**  
**Research Engineer**  
**LLM / NLP Engineer**  
**Applied AI Engineer**  
**AI Research Collaborations**

I am particularly interested in opportunities around:

**LLM systems · agents · memory · multilingual NLP · evaluation · inference · Physical AI · robotics**

[LinkedIn](https://linkedin.com/in/vishnup22) · [GitHub](https://github.com/vishnup22) · [Hugging Face](https://huggingface.co/pulipakav-1) · [Email](mailto:vishnupulipaka22@gmail.com)
