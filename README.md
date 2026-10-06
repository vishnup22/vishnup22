# Vishnu 

### AI Engineer · LLM Systems · AI Research

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=220&color=0:020617,45:0f172a,100:111827&text=Vishnu%20Pulipaka&fontColor=ffffff&fontSize=52&fontAlignY=38&desc=AI%20Engineer%20%E2%80%A2%20Researcher&descAlignY=58&descSize=20&animation=fadeIn" width="100%" />

<br>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=2800&pause=900&color=58A6FF&center=true&vCenter=true&width=800&lines=LLM+Systems+%E2%80%A2+Agents+%E2%80%A2+Memory;Multilingual+NLP+%E2%80%A2+Model+Evaluation;Efficient+Inference+%E2%80%A2+AI+Systems;Physical+AI+%E2%80%A2+Robotics+%E2%80%A2+Embodied+Intelligence" alt="Research Interests" />

<br><br>

<a href="https://github.com/vishnup22">
  <img src="https://img.shields.io/badge/GitHub-vishnup22-181717?style=for-the-badge&logo=github&logoColor=white">
</a>
<a href="https://huggingface.co/pulipakav-1">
  <img src="https://img.shields.io/badge/HuggingFace-pulipakav--1-FFD21E?style=for-the-badge&logo=huggingface&logoColor=000">
</a>
<a href="https://linkedin.com/in/vishnup22">
  <img src="https://img.shields.io/badge/LinkedIn-Vishnu%20Pulipaka-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white">
</a>
<a href="mailto:vishnupulipaka22@gmail.com">
  <img src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white">
</a>

</div>

<br>

## `> whoami`

I am an **AI Engineer and Researcher** working on systems that **reason, retrieve, remember, evaluate, and adapt**.

My work currently sits across:

```text
LLM Systems       → retrieval, agents, evaluation, post-training
Memory            → persistent context, retrieval, agent memory
Language Models   → multilingual + low-resource NLP
AI Systems        → inference, optimization, reliability
Research          → evaluation, fairness, retrieval stability
Physical AI       → robotics, embodied agents, perception → action
```

I am especially interested in where these areas begin to converge:

<div align="center">

### `Models × Memory × Agents × Perception × Action`

</div>

The question behind much of my work is simple:

> **How do we know an intelligent system actually became better — rather than simply becoming more complex?**

That is why I care deeply about **evaluation, reproducibility, failure analysis, and measurable system behavior**.

---

# 🧠 Research Directions

<table>
<tr>
<td width="50%" valign="top">

### 🧠 AI Memory

I am interested in AI systems that can accumulate useful experience instead of starting nearly from zero every interaction.

Areas I want to explore:

- episodic memory
- semantic memory
- working memory
- memory consolidation
- retrieval policies
- memory decay / forgetting
- shared multi-agent memory
- long-term personalized agents
- memory evaluation

**Core question**

> What should an intelligent system remember, retrieve, update, or deliberately forget?

</td>

<td width="50%" valign="top">

### 🤖 Physical AI

I am increasingly exploring intelligence beyond text-only environments.

Areas I am interested in:

- embodied agents
- robot learning
- Vision-Language-Action models
- multimodal foundation models
- world models
- robotic planning
- manipulation
- reinforcement learning
- simulation-to-real transfer
- robot memory

**Long-term direction**

> Connect perception, reasoning, memory, planning, and action inside the same intelligent system.

</td>
</tr>
</table>

---

# ⚡ Selected AI Systems

## 🔍 Production RAG Evaluation Platform

<a href="https://github.com/vishnup22/production-rag-eval-platform">
<img src="https://img.shields.io/badge/Repository-production--rag--eval--platform-238636?style=flat-square&logo=github">
</a>

An evaluation-first RAG platform designed to detect whether changes to retrieval or generation **actually improve the system**.

```text
Documents
    │
    ▼
┌───────────────┐
│   Retrieval   │
│  3 strategies │
└───────┬───────┘
        │
        ▼
┌───────────────┐
│     LLM       │
│  3 providers  │
└───────┬───────┘
        │
        ▼
┌─────────────────────────────┐
│         Evaluation          │
│                             │
│ Retrieval Hit Rate          │
│ Faithfulness                │
│ Answer Quality              │
│ Latency                     │
│ Regression Detection        │
└──────────────┬──────────────┘
               │
               ▼
        GitHub Actions Gate
```

**Current evaluation**

`100% retrieval hit rate` · `92% faithfulness`

Changes to prompts, retrieval configurations, or model behavior are evaluated through **CI regression gates** before being accepted.

> Treating RAG quality as a software regression problem.

---

## 🧩 FinSight AI — Multi-Agent Research System

<a href="https://github.com/vishnup22/FinSight-AI">
<img src="https://img.shields.io/badge/Repository-FinSight--AI-238636?style=flat-square&logo=github">
</a>

A four-agent asynchronous research system operating across **US, NSE, and BSE markets**.

```text
                        ┌────────────────┐
                        │   User Query   │
                        └───────┬────────┘
                                │
               ┌────────────────┼────────────────┐
               │                │                │
               ▼                ▼                ▼
         Research Agent   Sentiment Agent   Market Agent
               │                │                │
               └───────────┬────┴────────────────┘
                           ▼
                    Analysis Agent
                           │
                           ▼
                    LLM Evaluation
                           │
                           ▼
                  Portfolio Optimizer
```

Combines:

- asynchronous agent orchestration
- FinBERT sentiment
- structured reasoning
- LLM-as-judge evaluation
- Markowitz optimization

The research problem I care about here is not simply:

**“Can multiple agents talk?”**

It is:

**How do agent state, memory, handoffs, evaluation, and failure propagation affect the reliability of the final system?**

---

## 🌐 `tok-adapt`

<a href="https://github.com/vishnup22/tok-adapt">
<img src="https://img.shields.io/badge/Repository-tok--adapt-238636?style=flat-square&logo=github">
</a>

A Python library and CLI for adapting pretrained language models to **new languages and domains**.

```text
Tokenizer
    ↓
Vocabulary Adaptation
    ↓
Embedding Initialization
    ↓
Continued Pretraining
    ↓
Supervised Fine-Tuning
    ↓
DPO
```

### `CPT → SFT → DPO`

Supports:

`Tokenizer Expansion` · `Vocabulary Replacement` · `Embedding Adaptation` · `Weight Initialization` · `Continued Pretraining` · `SFT` · `DPO`

The broader research question is how **tokenization and representation capacity influence adaptation**, especially for languages poorly represented during pretraining.

---

## ⚙️ TensorRT Vision Inference

<a href="https://github.com/vishnup22/tensorrt-vision-server">
<img src="https://img.shields.io/badge/Repository-tensorrt--vision--server-238636?style=flat-square&logo=github">
</a>

A GPU inference study measuring the effect of TensorRT compilation on ResNet-50 serving performance.

<div align="center">

| | Result |
|---|---:|
| Throughput | **97 → 347 FPS** |
| Throughput gain | **3.55×** |
| P99 latency | **4.3× lower** |
| Accuracy loss | **0** |

</div>

Stack:

`PyTorch → ONNX → TensorRT 11 → FP16 → CUDA 12.4`

The focus is not only optimization.

It is understanding **where performance improvements come from and measuring them reproducibly**.

---

# 📚 Research

## 🌏 Dravidian Language Models

### Evaluating Dedicated Monolingual and Joint Multilingual Causal Models for Dravidian Languages

[![arXiv](https://img.shields.io/badge/arXiv-2608.07727-B31B1B?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2608.07727)
[![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github)](https://github.com/vishnup22/dravidian-lm-research)

Models and experiments across:

**తెలుగు Telugu · தமிழ் Tamil · ಕನ್ನಡ Kannada · മലയാളം Malayalam**

I study whether dedicated language models can outperform multilingual models when data and compute are constrained.

Evaluation spans:

```text
Language Modeling
├── Loss
├── Perplexity
└── Bits-per-byte

Tokenization
└── Tokenizer efficiency

Downstream Transfer
├── Sentiment
└── Named Entity Recognition
```

Compared against multilingual baselines including **mGPT, mBERT, and XLM-R**.

---

## ⚡ Reward Model Inference

### How Fast Can Reward Models Score?

[![arXiv](https://img.shields.io/badge/arXiv-2607.19712-B31B1B?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2607.19712)
[![Code](https://img.shields.io/badge/Code-GitHub-181717?style=flat-square&logo=github)](https://github.com/vishnup22/reward-model-benchmarks)

A systems study of reward-model inference for RLHF pipelines.

```text
PyTorch Eager
      │
      │ benchmark
      ▼
ONNX Runtime
      │
      ▼
Execution / Graph Analysis
```

The key finding:

> The observed CPU speedup is primarily explained by **ONNX Runtime execution and graph optimizations**, rather than C++ itself.

Research intersection:

`RLHF Infrastructure × Inference × Benchmarking × Systems Analysis`

---

## ⚖️ Release-Level Fairness Drift

<a href="https://github.com/vishnup22/fairness-drift-llms">
<img src="https://img.shields.io/badge/Code-fairness--drift--llms-181717?style=flat-square&logo=github">
</a>

A longitudinal evaluation framework for studying whether model fairness remains stable across releases.

<div align="center">

| Scope | Scale |
|---|---:|
| Model versions | **12** |
| Providers | **5** |
| Model families | **6** |
| Bias benchmarks | **7** |
| Evaluation examples | **~200K** |

</div>

The central idea:

> **Fairness should be regression-tested across model releases, not measured once and forgotten.**

**Status:** Under double-blind review.

---

## 🔐 Retrieval Stability

Researching **certifiable top-k retrieval stability under multi-agent communication**.

Datasets:

`HotpotQA` · `2WikiMultihopQA` · `MuSiQue`

The work studies whether retrieval rankings can remain stable under bounded perturbations introduced during agent communication.

```text
Original Query
      │
      ▼
   Retriever ──────────────► Top-k
      ▲
      │
Agent Communication
      │
      ▼
Perturbed Query
      │
      ▼
   Retriever ──────────────► Top-k'
                              │
                              ▼
                      Stability Certificate
```

Rather than asking only:

> Did retrieval change?

I am interested in:

> **Can we determine when retrieval is guaranteed not to change?**

---

# 🧠 Memory × Agents

This is one of the directions I want to push much deeper.

Modern agents can reason over impressive context lengths, but **context is not memory**.

I am interested in architectures where an agent develops persistent internal state across interactions:

```text
             ┌─────────────┐
             │   Working   │
             │    Memory   │
             └──────┬──────┘
                    │
       ┌────────────┼────────────┐
       ▼            ▼            ▼
   Episodic      Semantic     External
    Memory        Memory       Retrieval
       │            │            │
       └────────────┼────────────┘
                    ▼
              Agent Reasoning
                    │
                    ▼
                  Action
                    │
                    ▼
               Experience
                    │
                    └──────────► Memory Update
```

Questions I want to investigate:

- What deserves to become long-term memory?
- When should memory be retrieved?
- How should memories decay?
- How should contradictory memories be resolved?
- Can agents consolidate multiple experiences into abstractions?
- How should agent memory be benchmarked?
- How should memory operate in multi-agent systems?
- How does memory change long-horizon reasoning?

---

# 🤖 Physical AI

The direction I find most exciting is moving intelligence from:

```text
Prompt → Model → Response
```

toward:

```text
Perception
    ↓
World Understanding
    ↓
Memory
    ↓
Reasoning
    ↓
Planning
    ↓
Action
    ↓
Environment
    └──────────► New Experience
```

I am especially interested in:

<p align="center">

<img src="https://img.shields.io/badge/Embodied_AI-111827?style=for-the-badge">
<img src="https://img.shields.io/badge/Robot_Learning-111827?style=for-the-badge">
<img src="https://img.shields.io/badge/Vision_Language_Action-111827?style=for-the-badge">
<img src="https://img.shields.io/badge/World_Models-111827?style=for-the-badge">
<img src="https://img.shields.io/badge/Robot_Memory-111827?style=for-the-badge">
<img src="https://img.shields.io/badge/Reinforcement_Learning-111827?style=for-the-badge">

</p>

My long-term research interest is in systems that can **perceive, reason, remember previous interactions, plan, and act in physical environments**.

---

# 🧪 Research Philosophy

I like working across the full loop:

<div align="center">

### `BUILD → MEASURE → BREAK → UNDERSTAND → IMPROVE`

</div>

For me, a model benchmark is rarely the end of the project.

I want to know:

```text
Why did it improve?
Where does it fail?
Does the improvement generalize?
What changed internally?
What happens under distribution shift?
Can the result be reproduced?
Will the system remain reliable after the next change?
```

---

# 🛠 AI Stack

<div align="center">

### Models & Training

<img src="https://skillicons.dev/icons?i=python,pytorch" />

`Transformers` · `Sentence Transformers` · `SentencePiece`  
`CPT` · `SFT` · `DPO`

<br>

### LLM Systems

`RAG` · `Agents` · `Evaluation` · `LLM-as-Judge`  
`Retrieval` · `Structured Generation` · `Memory`

<br>

### Inference

<img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white">
<img src="https://img.shields.io/badge/TensorRT-76B900?style=for-the-badge&logo=nvidia&logoColor=white">
<img src="https://img.shields.io/badge/ONNX_Runtime-005CED?style=for-the-badge&logo=onnx&logoColor=white">

<br><br>

### AI Engineering

<img src="https://skillicons.dev/icons?i=fastapi,docker,githubactions" />

`MLflow` · `Prometheus` · `Evidently`

</div>

---

# 🔭 What I Want to Build Next

```text
                    Intelligent Systems
                           │
          ┌────────────────┼────────────────┐
          │                │                │
          ▼                ▼                ▼
        Models           Memory           Agents
          │                │                │
          └────────────────┼────────────────┘
                           ▼
                       Reasoning
                           │
              ┌────────────┴────────────┐
              ▼                         ▼
          Perception                  Planning
              │                         │
              └────────────┬────────────┘
                           ▼
                         Action
                           │
                           ▼
                     Physical World
```

I want to work toward AI systems that don't just produce better responses.

I want to understand how to build systems that can:

**reason · remember · adapt · learn · perceive · plan · act**

---

<div align="center">

## Let's Build

I am interested in **AI Engineer / Research Engineer opportunities** and research collaborations around:

`LLM Systems` · `Agents` · `Memory` · `Evaluation` · `Multilingual NLP` · `Efficient Inference` · `Physical AI` · `Robotics`

<br>

<a href="https://linkedin.com/in/vishnup22">
<img src="https://img.shields.io/badge/LinkedIn-Let's%20Connect-0A66C2?style=for-the-badge&logo=linkedin">
</a>

<a href="mailto:vishnupulipaka22@gmail.com">
<img src="https://img.shields.io/badge/Email-vishnupulipaka22%40gmail.com-EA4335?style=for-the-badge&logo=gmail">
</a>

<br><br>

<img src="https://komarev.com/ghpvc/?username=vishnup22&style=flat-square&label=PROFILE+VIEWS" />

</div>
