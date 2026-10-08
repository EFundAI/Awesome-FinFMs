# Awesome-FinFMs V2 🚀

<div align="center">

**A Living Review of Financial Foundation Models & Financial AI**

**V2 Curated: October 2026** · Reviewed & Updated Annually Every **December**

📄 [V1 Paper (Engineering'26)](./Survey_of_FFMs.pdf) · 📜 [V1 List (frozen)](./README_v1.md) · 🏷️ [V1 Tag](https://github.com/EFundAI/Awesome-FinFMs/releases/tag/v1.0-engineering)

</div>

> **What is this repo?** V1 was the static companion to our Engineering 2025 survey. **V2 is a dynamic, annually-reviewed living review**: it keeps the V1 classic list frozen, and incrementally tracks what has *actually happened* in financial AI at top venues since 2024 — new trends, new papers, new benchmarks, and the community event landscape.

---

## 🆕 What's New in V2

| | V1 (Engineering'25) | **V2 (Oct 2026)** |
|---|---|---|
| Scope | Foundation models (FinLFM / FinTSFM / FinVLFM) + data + applications | **+ 278 new papers** from AAAI / IJCAI / ICLR / ICML / KDD / WWW / ACL / EMNLP (main + Findings), 2024–2026 |
| Key finding | FFMs are emerging | **Domain-text pretraining has stalled**; the field has shifted to time-series FMs, agents, benchmarks, trustworthiness & ESG (see §New Trends) |
| Events | — | New **Community Events Calendar** (workshops & conferences) |
| Maintenance | Promised regular updates, but **no explicit mechanism** — remained largely static in practice | **Explicit annual December review** + rolling community contributions + public changelog |

**The big picture (2024 → 2026).** At top venues, new BloombergGPT/FinGPT-style *financial text foundation models* have essentially disappeared — the community consensus is that frontier general LLMs already match or beat domain-pretrained models on financial NLP. Research energy has migrated to eight active directions, which we use to organize the 278-paper collection below:

1. **Benchmarks & Evaluation** (largest cluster — an explosion of benchmarks covering nearly every financial task)
2. **Financial Time-Series & Event Foundation Models** (the *only* route where new "foundation models" still appear, e.g. Kronos)
3. **Agentic Finance** (trading / alpha-mining / investment agents — hottest application area in 2026)
4. **Trustworthiness, Safety, Fraud & Compliance**
5. **Financial Document Intelligence, QA & RAG**
6. **ESG & Sustainability**
7. **Multilingual & Low-Resource Financial NLP**
8. **Domain Adaptation & Training Paradigms** (how to adapt, not new pretraining)

---

## 📅 Community Events Calendar

### 🔬 Active Workshop Series

| Series | Host / SIG | Editions | Link | Status |
|---|---|---|---|---|
| **FinLLM @ IJCAI** | E Fund · Tsinghua · PolyU | IJCAI 2023 Macau → 2025 Montreal+Guangzhou → **2026 Bremen** | [finllm.github.io](https://finllm.github.io/workshop/#/) | 🟢 Active |
| **FinNLP** | ACL SIG-FinTech | 11 editions: IJCAI 2019/20/21/23 · EMNLP 2022 · IJCAI 2024 · COLING 2025 · EMNLP 2025(10th) → **EMNLP 2026 (11th)** | [sigfintech.github.io/finnlp2026](https://sigfintech.github.io/finnlp2026/) | 🟢 Active |
| **KDD MLF** (Machine Learning in Finance) | — | Annual since KDD 2018; **9th = KDD 2026 Jeju** | [KDD MLF](https://sites.google.com/view/kdd-mlf-2025) | 🟢 Active |
| **ICLR "Advances in Financial AI"** | — | 2025 Singapore (1st) → **2026 Rio (2nd, agentic + responsible AI theme)** | [ICLR 2026 FinAI](https://sites.google.com/view/iclr2026finai) | 🟢 Active |
| **AI4F** (LLMs & GenAI for Finance, @ ICAIF) | LinqAlpha et al. | ICAIF 2024 (1st) · 2025 · **2026 (3rd)** | [ai4f.org](https://ai4f.org) | 🟢 Active |
| **ICAIF Workshops** (umbrella) | ACM | 7 ws (2024) → 9 (2025) → **10 (2026)**: incl. AI4F, MFMB, QAI4Fin, RL4LLM-Agents, Financial AI Security… | [icaif2026.org/workshops](https://icaif2026.org/) | 🟢 Active |
| **NeurIPS "Generative AI in Finance"** | — | 2025 San Diego (1st) | [NeurIPS 2025](https://neurips.cc) | 🟡 New |
| **AAAI "Agentic AI in Financial Services"** | — | 2026 Singapore (1st) | [AAAI-26 WS](https://ai-4-finance.pages.dev) | 🟡 New |
| **FinIR @ SIGIR** | NTU / SMU | SIGIR 2020/21 → **2025 (rebooted: "in the era of GenAI")** | — | 🟢 Active |
| ~~ECONLP~~ | — | Merged into FinNLP joint workshops | — | ⚪ Absorbed |
| ~~FinWeb~~ (TheWebConf) | — | 2021–2023, discontinued | — | ⚪ Defunct |
| ~~NeurIPS FAIF series~~ | — | 2018–2020, discontinued | — | ⚪ Defunct |

### 🏛️ Key Conferences (financial AI presence)

- **ICAIF 2026** — 7th ACM Intl. Conf. on AI in Finance, **Nov 14–17, Milan (Bocconi)**. [icaif2026.org](https://icaif2026.org/)
- **AAAI / IJCAI** — growing financial LLM tracks (AAAI 2026 had 22 relevant papers incl. IAAI applied track)
- **KDD / TheWebConf** — fintech & quant-finance tracks growing (KDD 2026: 21 relevant papers)
- **ACL / EMNLP** — largest NLP venue cluster (127 papers 2024–2026); FinNLP workshop at EMNLP 2026
- **ICLR / ICML** — main battleground for time-series foundation models

---

## 🔥 New Trends 2024–2026: 278 Papers from Top Venues

> Collection methodology: four parallel sweeps (Oct 2026) covering all main-conference & Findings papers at **AAAI, IJCAI, ICLR, ICML, KDD, WWW, ACL, EMNLP (+NAACL/COLING/LREC-COLING)** 2024–2026, keyword-filtered for finance × LLM/foundation-model/agent/RAG paradigms, manually verified, all with official links. Pure traditional-DL finance papers (LSTM/CNN/GNN/RL stock prediction) are **excluded** by design. *Borderline* entries are marked.

### 1️⃣ Benchmarks & Evaluation *(largest cluster — the benchmark explosion)*

*Reasoning / math / multi-hop:*
- [FinanceMATH: Knowledge-Intensive Math Reasoning in Finance Domains](https://aclanthology.org/2024.acl-long.693/) (ACL'24)
- [BizBench: A Quantitative Reasoning Benchmark for Business and Finance](https://aclanthology.org/2024.acl-long.452/) (ACL'24)
- [DocFinQA: A Long-Context Financial Reasoning Dataset](https://aclanthology.org/2024.acl-short.42/) (ACL'24)
- [FCMR: Robust Evaluation of Financial Cross-Modal Multi-Hop Reasoning](https://aclanthology.org/2025.acl-long.1138/) (ACL'25)
- [FinanceReasoning: Benchmarking Financial Numerical Reasoning More Credible, Comprehensive and Challenging](https://aclanthology.org/2025.acl-long.766/) (ACL'25)
- [XFinBench: Benchmarking LLMs in Complex Financial Problem Solving and Reasoning](https://aclanthology.org/2025.findings-acl.457/) (ACL'25 Findings)
- [FinMathBench: A Formula-Driven Benchmark for Evaluating LLMs' Math Reasoning in Finance](https://doi.org/10.1609/aaai.v40i37.40358) (AAAI'26)
- [FinChain: A Symbolic Benchmark for Verifiable Chain-of-Thought Financial Reasoning](https://aclanthology.org/2026.acl-long.662/) (ACL'26)
- [Achieving Multi-Hop Calculation and Safe Abstention in Financial Numerical Reasoning by Metric Graph Constrained LLMs](https://aclanthology.org/2026.acl-long.1273/) (ACL'26)
- [AlphaQT-Bench: Diagnosing the Gap between Financial Code Generation and Quantitative Reasoning](https://aclanthology.org/2026.findings-acl.138/) (ACL'26 Findings)
- [RealFin: How Well Do LLMs Reason About Finance When Users Leave Things Unsaid?](https://aclanthology.org/2026.findings-acl.1255/) (ACL'26 Findings)
- [EconLogicQA: A Question-Answering Benchmark for Economic Sequential Reasoning](https://aclanthology.org/2024.findings-emnlp.125/) (EMNLP'24 Findings)
- [Fin-PRM: A Domain-Specialized Process Reward Model for Financial Reasoning](https://doi.org/10.24963/ijcai.2026/683) (IJCAI'26)

*General financial capability:*
- [Benchmarking LLMs on CFLUE](https://aclanthology.org/2024.findings-acl.337/) (ACL'24 Findings) · Chinese
- [FLaME: Financial Language Model Evaluation](https://aclanthology.org/2025.findings-acl.1164/) (ACL'25 Findings)
- [CFinBench: A Comprehensive Chinese Financial Benchmark](https://aclanthology.org/2025.naacl-long.40/) (NAACL'25) · Chinese
- [FinEval: A Chinese Financial Domain Knowledge Evaluation Benchmark](https://aclanthology.org/2025.naacl-long.318/) (NAACL'25) · Chinese
- [FinDABench: Benchmarking Financial Data Analysis Ability of LLMs](https://aclanthology.org/2025.coling-main.48/) (COLING'25)
- [FinSearchComp: Realistic, Expert-Level Evaluation of Financial Search and Reasoning](https://openreview.net/forum?id=8AJbbbe2ni) (ICLR'26, competition)
- [Fin-RATE: Real-world Financial Analytics and Tracking Evaluation on SEC Filings](https://doi.org/10.1145/3770855.3817528) (KDD'26)
- [EDINET-Bench: Evaluating LLMs on Complex Financial Tasks using Japanese Financial Statements](https://openreview.net/forum?id=Dxns0cj15A) (ICLR'26) · Japanese
- [BizFinBench.v2: Reliable LLMs in Finance via Real-User Data, Bilingual Evaluation](https://openreview.net/forum?id=8cQGYH64R2) (ICML'26)

*Multimodal:*
- [FinMME: Benchmark Dataset for Financial Multi-Modal Reasoning Evaluation](https://aclanthology.org/2025.acl-long.1426/) (ACL'25)
- [VisFinEval: Scenario-Driven Chinese Multimodal Financial Understanding](https://aclanthology.org/2025.emnlp-main.1229/) (EMNLP'25) · Chinese
- [CFMME: Chinese Financial Multimodal Evaluation](https://aclanthology.org/2026.acl-long.1000/) (ACL'26) · Chinese
- [FinChart-Bench: Financial Chart Comprehension in VLMs](https://aclanthology.org/2026.acl-long.615/) (ACL'26)
- [FinMMDocR: Financial Multimodal Reasoning — Scenario Awareness, Documents, Multi-Step Computation](https://doi.org/10.1609/aaai.v40i30.39785) (AAAI'26)
- [FinCall-Surprise: Large-Scale Multi-modal Benchmark for Earning Surprise Prediction](https://aclanthology.org/2026.acl-long.610/) (ACL'26)
- [Fin-Fact: Multimodal Financial Fact-Checking and Explanation Generation](https://doi.org/10.1145/3701716.3715292) (WWW'25)
- [VideoConviction: Multimodal Benchmark for Human Conviction and Stock Recommendations](https://doi.org/10.1145/3711896.3737417) (KDD'25)

*Agents & decision-making:*
- [INVESTORBENCH: Financial Decision-Making Tasks with LLM Agents](https://aclanthology.org/2025.acl-long.126/) (ACL'25)
- [CNFinBench: Expertise, Autonomy, Integrity in Finance (Chinese)](https://doi.org/10.1145/3770855.3817482) (KDD'26) · Chinese
- [BacktestBench: LLMs for Automated Quantitative Strategy Backtesting](https://doi.org/10.1145/3770855.3817460) (KDD'26)
- [AlphaForgeBench: End-to-End Trading Strategy Design with LLMs](https://doi.org/10.1145/3770855.3817500) (KDD'26)
- [AlphaBench: LLMs in Formulaic Alpha Factor Mining](https://openreview.net/forum?id=d97Q8r7ZKZ) (ICLR'26)
- [AlphaEval: Efficient Evaluation Framework for Formula Alpha Mining](https://doi.org/10.1145/3770855.3817727) (KDD'26)
- [ProFinR: Professional-Grade Financial Agents — Benchmarking, Tooling, Structured Reasoning](https://openreview.net/forum?id=x6nNQBumUQ) (ICML'26)
- [Agent Trading Arena: Numerical Understanding in LLM-Based Agents](https://aclanthology.org/2025.findings-emnlp.294/) (EMNLP'25 Findings)
- [Behavioral Consistency Validation for LLM Agents via Stock-Market Simulation](https://aclanthology.org/2026.findings-acl.2006/) (ACL'26 Findings)
- [From Tasks to Teams: Risk-First Evaluation of Multi-Agent LLM Systems in Finance](https://aclanthology.org/2026.findings-acl.1934/) (ACL'26 Findings)

*Trustworthiness-flavored benchmarks* (see also §4):
- [FinTrust: Trustworthiness Evaluation in Finance](https://aclanthology.org/2025.emnlp-main.512/) (EMNLP'25)
- [Fraud-R1: Robustness Against Augmented Fraud and Phishing Inducements](https://aclanthology.org/2025.findings-acl.226/) (ACL'25 Findings)
- [FinSafetyBench: LLM Safety in Real-World Financial Scenarios](https://aclanthology.org/2026.findings-acl.694/) (ACL'26 Findings)
- [Fin-Bias: LLM Decision-Making under Human Bias in Finance](https://aclanthology.org/2026.findings-acl.279/) (ACL'26 Findings)
- [ESG-Bench: Long-Context ESG Reports for Hallucination Mitigation](https://doi.org/10.1609/aaai.v40i46.41281) (AAAI'26)
- [Golden Touchstone: Bilingual (Zh/En) Financial LLM Benchmark](https://aclanthology.org/2025.findings-emnlp.1227/) (EMNLP'25 Findings)
- [Plutus: LLMs in Low-Resource Greek Finance](https://aclanthology.org/2025.emnlp-main.1535/) (EMNLP'25) · Greek
- [SAHM: Arabic Financial and Shari'ah-Compliant Reasoning](https://aclanthology.org/2026.acl-long.1593/) (ACL'26) · Arabic
- [MultiFinBen: Multilingual Multimodal Financial Applications](https://aclanthology.org/2026.acl-long.770/) (ACL'26)
- [FinMTEB: Finance Massive Text Embedding Benchmark](https://aclanthology.org/2025.emnlp-main.179/) (EMNLP'25)
- [MFinMeeting: Multilingual Multi-Sector Financial Meeting Understanding](https://aclanthology.org/2025.findings-acl.14/) (ACL'25 Findings)
- [InsLogicBench: Argumentation Logic for Insurance Claims Adjudication](https://aclanthology.org/2026.acl-long.1035/) (ACL'26)
- [TaxPraBen: Chinese Real-World Tax Practice Benchmark](https://aclanthology.org/2026.acl-long.1765/) (ACL'26) · Chinese
- [Finch: Finance & Accounting across Spreadsheet-Centric Workflows](https://aclanthology.org/2026.findings-acl.523/) (ACL'26 Findings)
- [ICFD-31k: Large-Scale Dataset for Real-Time Conversational Fraud Detection](https://doi.org/10.24963/ijcai.2026/786) (IJCAI'26, borderline)
- [CTBench: Cryptocurrency Time Series Generation Benchmark](https://openreview.net/forum?id=RzT2sombPD) (ICLR'26, borderline)
- [LOB-Bench: Benchmarking Generative AI on Limit Order Book Data](https://openreview.net/forum?id=CXPpYJpYXQ) (ICML'25)
- [DMind: Holistic LLM Assessment across Web3](https://doi.org/10.1145/3770855.3817512) (KDD'26, borderline)
- [OmniEval: Omnidirectional RAG Evaluation in Finance](https://aclanthology.org/2025.emnlp-main.292/) (EMNLP'25)
- [FinRAGBench-V: Multimodal RAG with Visual Citation](https://aclanthology.org/2025.emnlp-main.211/) (EMNLP'25)
- [FinMRAGBench: Realistic Multi-Modal RAG in Financial Documents](https://aclanthology.org/2026.findings-acl.187/) (ACL'26 Findings)
- [FinLFQA: Attributed Text Generation in Financial Long-Form QA](https://aclanthology.org/2025.findings-emnlp.908/) (EMNLP'25 Findings)
- [FinDVer: Explainable Claim Verification over Long Financial Documents](https://aclanthology.org/2024.emnlp-main.818/) (EMNLP'24)
- [Are LLMs Reliable Reviewers? Error Detection in Financial Documents](https://aclanthology.org/2026.findings-acl.1481/) (ACL'26 Findings)
- [What Factors Affect LLMs and RLLMs in Financial QA?](https://aclanthology.org/2026.findings-acl.752/) (ACL'26 Findings)
- [Position: Evaluating LLMs in Finance Requires Explicit Bias Consideration](https://openreview.net/forum?id=EDsAEXBFBk) (ICML'26, position)

### 2️⃣ Financial Time-Series & Event Foundation Models

*The only route where new "foundation models" still emerge:*
- [Kronos: A Foundation Model for the Language of Financial Markets](https://doi.org/10.1609/aaai.v40i30.39730) (AAAI'26) — K-line pretraining, 12B bars / 45 exchanges ⭐
- [TransactionGPT: Foundational Transaction Modeling](https://doi.org/10.1145/3770855.3818496) (KDD'26) — billion-scale real transactions
- [TREASURE: Transformer Foundation Model for High-Volume Transaction Understanding](https://doi.org/10.1145/3770854.3783942) (KDD'26)
- [A Foundation Model for Multimodal Event Sequences in Financial Applications](https://doi.org/10.1145/3770855.3818311) (KDD'26)
- [Pre-training Time Series Models with Stock Data Customization](https://doi.org/10.1145/3711896.3737005) (KDD'25)
- [CI-STHPAN: Pre-trained Attention Network for Stock Selection](https://doi.org/10.1609/aaai.v38i8.28770) (AAAI'24, borderline)

*General-purpose TSFMs (backbones validated on financial data):*
- [Moirai: Unified Training of Universal Time Series Forecasting Transformers](https://proceedings.mlr.press/v235/woo24a.html) (ICML'24)
- [MOMENT: A Family of Open Time-Series Foundation Models](https://proceedings.mlr.press/v235/goswami24a.html) (ICML'24)
- [Timer: Generative Pre-trained Transformers Are Large Time Series Models](https://proceedings.mlr.press/v235/liu24cb.html) (ICML'24)
- [Time-MoE: Billion-Scale Time Series Foundation Models with MoE](https://openreview.net/forum?id=e1wDDFmlVu) (ICLR'25)
- [Timer-XL: Long-Context Transformers for Unified Time Series Forecasting](https://openreview.net/forum?id=L9eBxTCpQG) (ICLR'25)
- [Sundial: Highly Capable Time Series Foundation Models](https://openreview.net/forum?id=LO7ciRpjI5) (ICML'25)
- [Moirai-MoE: TSFMs with Sparse Mixture of Experts](https://openreview.net/forum?id=SrEOUSyJcR) (ICML'25)

*LLM × time-series methods:*
- [Time-LLM: Time Series Forecasting by Reprogramming LLMs](https://openreview.net/forum?id=Unb5CVPtae) (ICLR'24)
- [LangTime: Language-Guided Unified Model for Time Series with PPO](https://openreview.net/forum?id=VfoKOD65Zq) (ICML'25, borderline)
- [Multi-Scale Hypergraph Meets LLMs for Time Series Analysis](https://openreview.net/forum?id=SbBX2dCw3y) (ICLR'26)
- [Reasoning on Time-Series for Financial Technical Analysis (VTA)](https://openreview.net/forum?id=PcjIe5xNaY) (ICLR'26)
- [TimeOmni-1: Incentivizing Complex Reasoning with Time Series in LLMs](https://openreview.net/forum?id=kOIclg7muL) (ICLR'26)

*Market simulation & generative market modeling:*
- [MarS: Financial Market Simulation Engine Powered by Generative FM](https://openreview.net/forum?id=Yqk7EyT52H) (ICLR'25)
- [MarketSim: Simulating Stock Markets with Large-Scale Generative Agents](https://openreview.net/forum?id=EzpJxPDqXB) (ICML'26)
- [CoFinDiff: Controllable Financial Diffusion for Time Series Generation](https://doi.org/10.24963/ijcai.2025/1040) (IJCAI'25, borderline)
- [DiffLOB: Diffusion Counterfactual Generation in Limit Order Books](https://doi.org/10.24963/ijcai.2026/730) (IJCAI'26, borderline)
- [Controllable Financial Market Generation with Diffusion Guided Meta Agent](https://doi.org/10.1609/aaai.v40i1.37009) (AAAI'26, borderline)

*Critical / analysis studies (what's broken & why):*
- [Understanding the Implicit Biases of Design Choices for TSFMs](https://openreview.net/forum?id=5jkzTzV5Ao) (ICLR'26, borderline)
- [Beyond Accuracy: Are TSFMs Well-Calibrated?](https://openreview.net/forum?id=nGBN7UjHcy) (ICLR'26, borderline)
- [When Foundation Models are One-Liners: Limitations for TS Anomaly Detection](https://openreview.net/forum?id=H27kvyG4qf) (ICLR'26, borderline)
- [Position: TSFMs Require Explicit Domain-Level Benchmarks](https://openreview.net/forum?id=W2eEMPjzIQ) (ICML'26, position, borderline)
- [Understanding Transformers for TS Forecasting: A Case Study on Moirai](https://openreview.net/forum?id=iAPSx90gwJ) (ICLR'26, borderline)
- [Universal Redundancies in TSFMs](https://openreview.net/forum?id=DyA4KHj1wy) (ICML'26, borderline)
- [AdaPTS: Adapting Univariate FMs to Probabilistic Multivariate Forecasting](https://openreview.net/forum?id=yeICCRy3lE) (ICML'25, borderline)
- [In-Context Fine-Tuning for TSFMs](https://openreview.net/forum?id=uxzgGLWPj2) (ICML'25, borderline)
- [CoRA: Correlation-aware Adapter for Multivariate TSFM](https://openreview.net/forum?id=JRlNrcTllN) (ICLR'26, borderline)
- [Zeus: Tuning-Free Foundation Model for Time Series](https://openreview.net/forum?id=Dtue4WLYSk) (ICML'26, borderline)
- [Mantis: Lightweight FM for Time Series Classification](https://openreview.net/forum?id=gbJMAjXLZ4) (ICML'26, borderline)
- [Olivia: Harmonizing TSFMs with Power Spectral Density](https://openreview.net/forum?id=F5ULzUwZrv) (ICML'26, borderline)
- [FeDaL: Federated Dataset Learning for General TSFMs](https://openreview.net/forum?id=HK6t5x5gJq) (ICLR'26, borderline)
- [UniCA: Unified Covariate Adaptation for TSFM](https://openreview.net/forum?id=I8q4MZb4OP) (ICLR'26, borderline)
- [CauKer: Classification TSFMs Pretrained on Synthetic Data](https://openreview.net/forum?id=xBW2FIfswU) (ICLR'26, borderline)
- [See More, Forecast Better and Faster (SPRINT)](https://openreview.net/forum?id=Ql4P9hu3Pa) (ICML'26, borderline)
- [Channel Adapter for Zero-Shot Multivariate TSFM (ChaTSFM)](https://openreview.net/forum?id=OJriSoFuDq) (ICML'26, borderline)
- [Time-PEFT: Complexity-Based Fine-Tuning for TSFMs](https://openreview.net/forum?id=n8seTOinYs) (ICML'26, borderline)
- [Consensus Subspace Distillation for TSFMs](https://openreview.net/forum?id=66l0POQkge) (ICML'26, borderline)
- [Aurora: Universal Generative Multimodal Time Series Forecasting](https://openreview.net/forum?id=VVJ6Ck9JBl) (ICLR'26)
- [Towards FMs for Zero-Shot TS Anomaly Detection via Synthetic Data](https://openreview.net/forum?id=yXqnyIvGAy) (ICML'26, borderline)
- [Adaptive Conformal Anomaly Detection with TSFMs](https://openreview.net/forum?id=7uFbs68MSI) (ICLR'26, borderline)
- [Complexity- and Statistics-Guided Anomaly Detection in TSFMs](https://openreview.net/forum?id=rBt9aW3Mx7) (ICLR'26, borderline)
- [Test-Time Efficient Pretrained Model Portfolios for TS Forecasting](https://openreview.net/forum?id=iqUMjxfDNH) (ICLR'26, borderline)
- [Adapt Data to Model for Domain-Shared TSFMs](https://openreview.net/forum?id=uTK1SNgi1N) (ICLR'26, borderline)
- [Enhancing TSFMs via Wavelet-based Tokenization](https://openreview.net/forum?id=B6WalMoQJW) (ICML'25, borderline)
- [Lightweight Online Adaption for TSFM Forecasts](https://openreview.net/forum?id=gAxYbvoOQz) (ICML'25, borderline)
- [Exploring Representations and Interventions in TSFMs](https://openreview.net/forum?id=goVzfYtj58) (ICML'25, borderline)
- [Position: What Can LLMs Tell Us about Time Series Analysis](https://proceedings.mlr.press/v235/jin24i.html) (ICML'24, position, borderline)
- [Multi-Patch Prediction: Adapting LMs for TS Representation (aLLM4TS)](https://proceedings.mlr.press/v235/bian24a.html) (ICML'24, borderline)

*Financial event/text-time fusion:*
- [GS-Fuse: Granger-Supervised Gated Fusion for Event-Driven Financial Forecasting](https://doi.org/10.1145/3770855.3817927) (KDD'26, borderline)
- [FinRipple: Aligning LLMs with Financial Market Event Ripple Effects](https://aclanthology.org/2025.findings-acl.489/) (ACL'25 Findings)
- [ITFormer: Bridging Time Series and Natural Language for Multi-Modal QA](https://openreview.net/forum?id=GByP03IitA) (ICML'25, borderline)
- [Time-VLM: Multimodal VLMs for Augmented Time Series Forecasting](https://openreview.net/forum?id=b5h60xQnzM) (ICML'25, borderline)
- [Time Series, Vision, and Language: Limits of Alignment in Contrastive Spaces](https://openreview.net/forum?id=TQi2IqvpIf) (ICML'26, borderline)

### 3️⃣ Agentic Finance *(hottest application area in 2026)*

*Trading & investment agents:*
- [A Multimodal Foundation Agent for Financial Trading](https://doi.org/10.1145/3637528.3671801) (KDD'24)
- [CryptoTrade: Reflective LLM Agent for Zero-Shot Cryptocurrency Trading](https://aclanthology.org/2024.emnlp-main.63/) (EMNLP'24)
- [HedgeAgents: Balanced-Aware Multi-Agent Financial Trading](https://doi.org/10.1145/3701716.3715232) (WWW'25)
- [FLAG-TRADER: Fusion LLM-Agent with Gradient-Based RL for Trading](https://aclanthology.org/2025.findings-acl.716/) (ACL'25 Findings)
- [QuantAgents: Towards Multi-Agent Financial System via Simulated Trading](https://aclanthology.org/2025.findings-emnlp.945/) (EMNLP'25 Findings)
- [Automate Strategy Finding with LLM in Quant Investment](https://aclanthology.org/2025.findings-emnlp.1005/) (EMNLP'25 Findings)
- [FinHEAR: Human Expertise + Risk-Aware Temporal Reasoning for Financial Decisions](https://aclanthology.org/2025.findings-emnlp.87/) (EMNLP'25 Findings)
- [Trade in Minutes! Rationality-Driven Agentic System for Quant Trading](https://openreview.net/forum?id=ROEwZAxqyS) (ICLR'26)
- [AlphaQuanter: End-to-End Tool-Augmented Agentic RL for Stock Trading](https://aclanthology.org/2026.findings-acl.456/) (ACL'26 Findings)
- [PortfolioPilot: Agentic Platform for Portfolio Management](https://doi.org/10.1609/aaai.v40i48.42396) (AAAI'26, IAAI)
- [Agentic Solutions for IT Financial Operations](https://doi.org/10.1609/aaai.v40i48.42387) (AAAI'26, IAAI)

*Alpha / factor mining agents:*
- [LLMFactor: Extracting Profitable Factors through Prompts](https://aclanthology.org/2024.findings-acl.185/) (ACL'24 Findings)
- [Can LLMs Mine Interpretable Financial Factors? Neural-Symbolic Factor Mining Agent](https://aclanthology.org/2024.findings-acl.233/) (ACL'24 Findings)
- [AlphaAgent: LLM-Driven Alpha Mining with Regularized Exploration](https://doi.org/10.1145/3711896.3736838) (KDD'25)
- [AlphaAgentEvo: Self-Evolving Agentic RL for Alpha Mining](https://openreview.net/forum?id=lNmZrawUMu) (ICLR'26)
- [FactorMiner: Self-Evolving Agent with Skills and Experience Memory](https://doi.org/10.1145/3770855.3818978) (KDD'26)
- [AlphaMaster: Dual-Chain Feedback for Scalable Alpha Discovery](https://doi.org/10.1145/3770855.3818120) (KDD'26)

*Rigorous evaluation / falsification of LLM trading:*
- [Can LLM-based Financial Investing Strategies Outperform the Market in the Long Run? (FINSABER)](https://doi.org/10.1145/3770854.3785702) (KDD'26) ⭐
- [Global Merger-Arbitrage Forecasting with Language Models](https://openreview.net/forum?id=wDaX9bFufS) (ICML'26)

*Investment analysis & research agents:*
- [FinRpt: Dataset, Evaluation & LLM Multi-Agent Framework for Equity Research Reports](https://doi.org/10.1609/aaai.v40i1.37014) (AAAI'26)
- [Beyond Isolated Investor: Predicting Startup Success via Roleplay Collective Agents](https://doi.org/10.24963/ijcai.2026/721) (IJCAI'26)
- [Analyze Like a Venture Capitalist: Info-Gain & Knowledge Graph Reasoning for Startup Success](https://aclanthology.org/2026.findings-acl.1555/) (ACL'26 Findings, borderline)
- [FinSight: Towards Real-World Financial Deep Research](https://aclanthology.org/2026.acl-long.265/) (ACL'26)
- [Cogito: Cognitive Agentic Framework via Dynamic Graph of Thoughts for Financial Report Generation](https://aclanthology.org/2026.findings-acl.430/) (ACL'26 Findings)
- [InvestAlign: Aligning LLMs with Investor Decision-Making under Herd Behavior](https://aclanthology.org/2025.acl-long.495/) (ACL'25)

*Economic & market simulation with agents:*
- [MALLES: Multi-Agent LLM Economic Sandbox with Consumer Preference Alignment](https://doi.org/10.1145/3770855.3818824) (KDD'26, borderline)
- [Think, Speak, Decide: Language-Augmented MARL for Economic Decision-Making](https://doi.org/10.1609/aaai.v40i35.40201) (AAAI'26, borderline)
- [From Heard to Lived Opinions: LLM Agents Opinion Dynamics in Economic Environments](https://aclanthology.org/2026.findings-acl.580/) (ACL'26 Findings, borderline)
- [Market-Bench: LLMs on Economic and Trade Competition](https://aclanthology.org/2026.acl-long.1853/) (ACL'26, borderline)

*Surveys:*
- [Large Language Model Agents in Finance: A Survey Bridging Research, Practice, and Deployment](https://aclanthology.org/2025.findings-emnlp.972/) (EMNLP'25 Findings)

### 4️⃣ Trustworthiness, Safety, Fraud & Compliance

*Fraud detection:*
- [ScamNet: Explainable LLM-Based Fraudulent Shopping Website Detection](https://doi.org/10.1609/aaai.v39i27.35000) (AAAI'25)
- [DGP: Dual-Granularity Prompting with Graph-Enhanced LLMs for Fraud Detection](https://doi.org/10.1609/aaai.v40i18.38541) (AAAI'26)
- [Targeting Borderline Fraudsters: Multi-View Hypergraph Fraud Detection with LLM-Guided Contrastive Learning](https://doi.org/10.1609/aaai.v40i18.38588) (AAAI'26)
- [FLAG: Fraud Detection with LLM-Enhanced GNN](https://doi.org/10.1145/3711896.3737220) (KDD'25)
- [Understanding Structured Financial Data with LLMs: A Fraud Detection Case Study](https://aclanthology.org/2026.acl-long.1071/) (ACL'26)
- [SAFE-QAQ: Slow-Thinking Audio-Text Fraud Detection via RL](https://aclanthology.org/2026.acl-long.1201/) (ACL'26, borderline)
- [CAMERA: Adapting to Semantic Camouflage in Text-Attributed Graph Fraud Detection](https://doi.org/10.24963/ijcai.2026/328) (IJCAI'26, borderline)
- [SHERLOCK: Dynamic Knowledge Adaptation in LLM-Enhanced E-commerce Risk Management](https://doi.org/10.1145/3770855.3818480) (KDD'26, borderline)
- [ChiFraud: Long-Term Web Text Dataset for Chinese Fraud Detection](https://aclanthology.org/2025.coling-main.398/) (COLING'25, borderline)
- [Online Fraud Detection via Test-Time Retrieval-Based Representation Enrichment](https://doi.org/10.1609/aaai.v39i12.33359) (AAAI'25, borderline)

*Security & manipulation:*
- [Learning to Conceal Risk: Controllable Multi-turn Red Teaming for LLMs in Finance](https://aclanthology.org/2026.acl-long.1903/) (ACL'26)
- [Web Fraud Attacks Against LLM-Driven Multi-Agent Systems](https://aclanthology.org/2026.findings-acl.686/) (ACL'26 Findings, borderline)
- [When AI Agents Collude Online: Financial Fraud Risks by Collaborative LLM Agents](https://openreview.net/forum?id=a1d2smwmBS) (ICLR'26)
- [Semantics-Preserving Adversarial Attacks on Event-Driven Stock Prediction](https://doi.org/10.1609/aaai.v40i44.41099) (AAAI'26, borderline)
- [FraudShield: Knowledge-Graph Defense for LLMs against Fraud Attacks](https://doi.org/10.1145/3774904.3792199) (WWW'26)

*Compliance, tax & regulation:*
- [Compliance-to-Code: Enhancing Financial Compliance Checking via Code Generation](https://doi.org/10.1145/3770854.3785703) (KDD'26)
- [Can LLMs Identify Tax Abuse?](https://doi.org/10.1609/aaai.v40i45.41165) (AAAI'26)
- [Language Models and Logic Programs for Trustworthy Tax Reasoning](https://doi.org/10.1609/aaai.v40i45.41212) (AAAI'26)
- [TaxReasoning: Benchmarking Knowledge-Intensive Math Reasoning with Evolving Tax Laws](https://doi.org/10.1609/aaai.v40i37.40367) (AAAI'26, borderline)
- [AI4Contracts: LLM & RAG-Powered Encoding of Financial Derivative Contracts](https://doi.org/10.24963/ijcai.2025/1034) (IJCAI'25)
- [RAG-Enhanced Evidence Recommendation in Financial Legal Resolutions](https://doi.org/10.1145/3701716.3715520) (WWW'25)
- [Harmful Terms and Where to Find Them: Unfavorable Financial Terms in Shopping Websites](https://doi.org/10.1145/3696410.3714573) (WWW'25)
- [A Guardrail Framework for Sensitive Financial Information Protection](https://doi.org/10.1609/aaai.v40i47.41498) (AAAI'26, borderline)
- [From Complexity to Clarity: AI/NLP's Role in Regulatory Compliance (survey)](https://aclanthology.org/2025.findings-acl.1366/) (ACL'25 Findings, borderline)
- [Interpreting Fedspeak: LLM Uncertainty-Aware Framework for Monetary Policy](https://doi.org/10.1609/aaai.v40i40.40739) (AAAI'26)

*Risk & credit:*
- [Think-like-LSTM: Memory-Augmented LLMs for Financial Risk Assessment (FraLLM)](https://doi.org/10.1145/3770855.3818491) (KDD'26)
- [Accept or Deny? LLM Fairness in Loan Approval across Table-to-Text Serialization](https://aclanthology.org/2025.findings-emnlp.947/) (EMNLP'25 Findings)
- [Translating Latent Representations for Money Laundering Detection](https://doi.org/10.24963/ijcai.2026/723) (IJCAI'26, borderline)
- [IGT4ETH: Isotropic Pre-trained Graph Transformer for Ethereum Account Classification](https://doi.org/10.1609/aaai.v40i28.39536) (AAAI'26, borderline)
- [Dual Pairwise Pre-training for Interbank Credit Rating](https://doi.org/10.1145/3696410.3714530) (WWW'25, borderline)
- [ZipZap: Efficient Training of LMs for Large-Scale Fraud Detection on Blockchain](https://doi.org/10.1145/3589334.3645352) (WWW'24, borderline)

### 5️⃣ Financial Document Intelligence, QA & RAG

*Financial QA & document understanding:*
- [FinTextQA: A Dataset for Long-form Financial Question Answering](https://aclanthology.org/2024.acl-long.328/) (ACL'24)
- [Fine-Tuning Smaller LMs for QA over Financial Documents](https://aclanthology.org/2024.findings-emnlp.617/) (EMNLP'24 Findings, borderline)
- [Hierarchical Retrieval with Evidence Curation for Open-Domain Financial QA](https://aclanthology.org/2025.findings-acl.855/) (ACL'25 Findings)
- [David vs. Goliath: Cost-Efficient Financial QA via Cascaded Multi-Agent Reasoning](https://aclanthology.org/2025.findings-emnlp.225/) (EMNLP'25 Findings)
- [FinCARDS: Card-Based Analyst Reranking for Financial Document QA](https://aclanthology.org/2026.findings-acl.1244/) (ACL'26 Findings)
- [Fin-STAR: Structure-as-Semantics to Resolve Implicitness in Financial Retrieval](https://aclanthology.org/2026.findings-acl.2151/) (ACL'26 Findings)
- [FinGEAR: Financial Mapping-Guided Enhanced Answer Retrieval](https://aclanthology.org/2025.findings-emnlp.382/) (EMNLP'25 Findings)

*Long-document & numerical robustness:*
- [NumCache: KV Cache Compression and Retrieval for Financial Document QA](https://doi.org/10.1145/3770855.3818131) (KDD'26)
- [Fighting Numerical Hallucinations via Data-centric Compilation for Online Financial QA](https://doi.org/10.1145/3770855.3818407) (KDD'26)
- [VeritasFi: Multi-tiered RAG for Multi-modal Financial QA](https://doi.org/10.1145/3774904.3792795) (WWW'26)
- [Data-Driven Function Calling in LLM for Online Financial QA](https://doi.org/10.1145/3774904.3792813) (WWW'26)

*Report & narrative generation:*
- [KAHAN: Knowledge-Augmented Hierarchical Analysis and Narration for Financial Data](https://aclanthology.org/2025.findings-emnlp.1405/) (EMNLP'25 Findings)
- [Prompting for Numerical Sequences: Market Comment Generation](https://aclanthology.org/2024.lrec-main.1155/) (LREC-COLING'24)
- [From Facts to Insights: LLM Generation & Evaluation of Earnings-Call Analytical Reports](https://aclanthology.org/2025.coling-main.705/) (COLING'25)
- [TermGPT: Multi-Level Contrastive Fine-Tuning for Terminology in Legal & Financial Domains](https://doi.org/10.1609/aaai.v40i2.37075) (AAAI'26)

*Contract / RFQ / structured-text parsing:*
- [Chat2Trade: Automating Financial RFQ Parsing with Fine-Tuned LLMs](https://doi.org/10.1145/3770854.3783923) (KDD'26)
- [Parameter-Efficient Instruction Tuning for Extreme Financial Numeral Labelling (XBRL)](https://aclanthology.org/2024.naacl-long.410/) (NAACL'24)

### 6️⃣ ESG & Sustainability

- [ESG Accountability Made Easy: DocQA at Your Service](https://doi.org/10.1609/aaai.v38i21.30574) (AAAI'24, IAAI, borderline)
- [Towards Robust ESG Analysis Against Greenwashing Risks: Aspect-Action Analysis](https://aclanthology.org/2025.acl-long.723/) (ACL'25)
- [ESGenius: Benchmarking LLMs on ESG and Sustainability Knowledge](https://aclanthology.org/2025.emnlp-main.739/) (EMNLP'25)
- [ESG-Bench: Long-Context ESG Reports for Hallucination Mitigation](https://doi.org/10.1609/aaai.v40i46.41281) (AAAI'26)
- [Learning the ESG Geometry with Domain-Aware Language Models](https://openreview.net/forum?id=CydNEMsNM6) (ICML'26)
- [ESG-Kor: Korean Dataset for ESG Information Extraction](https://aclanthology.org/2024.findings-emnlp.387/) (EMNLP'24 Findings, borderline)

### 7️⃣ Multilingual & Low-Resource Financial NLP

- [Dólares or Dollars? Bilingual Financial LLMs between Spanish and English](https://doi.org/10.1145/3637528.3671554) (KDD'24) · Spanish-English
- [IndicFinNLP: Financial NLP for Indian Languages](https://aclanthology.org/2024.lrec-main.789/) (LREC-COLING'24, borderline)
- [FinCorpus-DE10k: German Financial Domain Corpus](https://aclanthology.org/2024.lrec-main.639/) (LREC-COLING'24, borderline)
- [EFSA: Event-Level Financial Sentiment Analysis (Chinese)](https://aclanthology.org/2024.acl-long.402/) (ACL'24) · Chinese
- [OEE-CFC: Open Event Extraction from Chinese Financial Commentary](https://aclanthology.org/2024.findings-emnlp.256/) (EMNLP'24 Findings, borderline) · Chinese
- [Benchmarking LLMs on CFLUE (Chinese)](https://aclanthology.org/2024.findings-acl.337/) (ACL'24 Findings) · Chinese
- [FinEval & CFinBench (Chinese benchmarks)](https://aclanthology.org/2025.naacl-long.318/) (NAACL'25) · Chinese
- [VisFinEval: Chinese Multimodal Financial Understanding](https://aclanthology.org/2025.emnlp-main.1229/) (EMNLP'25) · Chinese
- [Golden Touchstone: Bilingual (Zh/En) Financial LLM Benchmark](https://aclanthology.org/2025.findings-emnlp.1227/) (EMNLP'25 Findings)
- [Plutus: Low-Resource Greek Finance](https://aclanthology.org/2025.emnlp-main.1535/) (EMNLP'25) · Greek
- [Translating Domain Terminology in Tax & Financial Education](https://aclanthology.org/2025.emnlp-main.1774/) (EMNLP'25, borderline)
- [CFMME: Chinese Financial Multimodal Evaluation](https://aclanthology.org/2026.acl-long.1000/) (ACL'26) · Chinese
- [MultiFinBen: Multilingual Multimodal Financial Applications](https://aclanthology.org/2026.acl-long.770/) (ACL'26)
- [SAHM: Arabic Financial & Shari'ah-Compliant Reasoning](https://aclanthology.org/2026.acl-long.1593/) (ACL'26) · Arabic
- [TaxPraBen: Chinese Real-World Tax Practice](https://aclanthology.org/2026.acl-long.1765/) (ACL'26) · Chinese
- [FIND: Multimodal Financial Reasoning for Indic Languages](https://aclanthology.org/2026.findings-acl.1639/) (ACL'26 Findings) · Indic
- [EDINET-Bench: Japanese Financial Statements](https://openreview.net/forum?id=Dxns0cj15A) (ICLR'26) · Japanese
- [Economy Watchers Survey: Japanese Financial Domain Datasets](https://doi.org/10.1145/3701716.3715304) (WWW'25, borderline) · Japanese

### 8️⃣ Domain Adaptation & Training Paradigms *(how to adapt, not new pretraining)*

*Post-training & domain specialization studies:*
- [Demystifying Domain-adaptive Post-training for Financial LLMs](https://aclanthology.org/2025.emnlp-main.1579/) (EMNLP'25)
- [Multi-perspective Analysis of LLM Domain Specialization: Accounting Audit Procedures](https://aclanthology.org/2025.emnlp-main.891/) (EMNLP'25)
- [Parameter Efficient Instruction Tuning of LLMs for Financial Applications](https://www.ijcai.org/proceedings/2024/962) (IJCAI'24)
- [TermGPT: Multi-Level Contrastive Fine-Tuning for Terminology Adaptation](https://doi.org/10.1609/aaai.v40i2.37075) (AAAI'26)

*Efficient & specialized encoders (the "small vs. large" debate):*
- [FinBERT2: Specialized Bidirectional Encoder for Finance-Specific Deployment](https://doi.org/10.1145/3711896.3737219) (KDD'25, borderline)
- [Efficient Multi-Expert Tabular Language Model for Banking](https://doi.org/10.1145/3690624.3709400) (KDD'25)
- [Fine-Tuning Smaller Language Models for QA over Financial Documents](https://aclanthology.org/2024.findings-emnlp.617/) (EMNLP'24 Findings, borderline)

*Domain LLMs & applications of general models in finance:*
- [FinTral: A Family of GPT-4 Level Multimodal Financial LLMs](https://aclanthology.org/2024.findings-acl.774/) (ACL'24 Findings)
- [Ploutos: Explainable Stock Movement Prediction with Financial LLM](https://doi.org/10.1145/3701716.3715254) (WWW'25)
- [MERA: Mixture of Experts with Retrieval-Augmented Representation for Stock Patterns](https://doi.org/10.1145/3701716.3715513) (WWW'25)
- [Pre-Finetuning with Impact Duration Awareness for Stock Movement Prediction](https://doi.org/10.1145/3701716.3715551) (WWW'25, borderline)
- [Can LLMs Follow Concept Annotation Guidelines? Scientific & Financial Domains](https://aclanthology.org/2024.findings-acl.478/) (ACL'24 Findings, borderline)
- [LLMs as Financial Data Annotators: Effectiveness and Efficiency](https://aclanthology.org/2024.lrec-main.885/) (LREC-COLING'24)

*LLM behavior & economics-of-AI studies:*
- [STEER: Assessing the Economic Rationality of LLMs](https://proceedings.mlr.press/v235/raman24b.html) (ICML'24)
- [Are LLMs Rational Investors? Financial Bias in LLMs](https://aclanthology.org/2025.findings-acl.1239/) (ACL'25 Findings)
- [Evaluating and Aligning Human Economic Risk Preferences in LLMs](https://aclanthology.org/2025.emnlp-main.917/) (EMNLP'25, borderline)
- [Language Models Trained to do Arithmetic Predict Human Risky Choice](https://openreview.net/forum?id=Tn8EQIFIMQ) (ICLR'25, borderline)
- [Lost in Prediction: Why Social Media Narratives Don't Help Macroeconomic Forecasting](https://openreview.net/forum?id=zFAhRlklbb) (ICLR'25, borderline)
- [EconNLI: Evaluating LLMs on Economics Reasoning](https://aclanthology.org/2024.findings-acl.58/) (ACL'24 Findings, borderline)
- [Towards the Terminator Economy: Assessing Job Exposure to AI Through LLMs](https://doi.org/10.24963/ijcai.2025/1066) (IJCAI'25, borderline)

---

## 🏛️ Classic Foundations (V1)

The V1 list — the Engineering'25 survey companion covering **Financial Language / Time-Series / Visual-Language Foundation Models, datasets, and applications** (the era of FinBERT → BloombergGPT → FinGPT → PIXIU → XuanYuan) — is preserved **frozen** here:

👉 **[README_v1.md](./README_v1.md)** · 🏷️ **[v1.0-engineering tag](https://github.com/EFundAI/Awesome-FinFMs/releases/tag/v1.0-engineering)** · 📄 **[Survey PDF](./Survey_of_FFMs.pdf)**

V1 remains the authoritative catalog for the *foundation-model era* (≈2019–2024). V2's §1–§8 above are the *increment* on top of it.

---

## 🔁 Maintenance: A Living Review

- **Curated** October 2026 (collection sweeps run 2026-10-07; 278 papers verified with official links).
- **Reviewed & updated every December** — the annual review scans the just-finished conference cycle (e.g., Dec 2026 review adds EMNLP 2026, NeurIPS 2026, ICAIF 2026 proceedings + next-year workshop deadlines) and updates trend conclusions if the landscape shifts.
- Each December review bumps the **"last reviewed"** date above and appends to the [changelog](#changelog) below.

### Changelog
| Date | Event |
|---|---|
| 2025 | V1 released with the Engineering survey |
| **2026-10** | **V2 launched**: V1 frozen (tag `v1.0-engineering`), +278 papers (2024–2026) in 8 trend categories, community events calendar, annual-review mechanism |

---

## 🤝 Contributing

We welcome community contributions to keep this a truly **living** review:

- **New papers** — submit an issue/PR with title, venue & year, official link, one-line summary, and the §1–§8 category you propose.
- **Corrections** — miscategorized / wrong link / missing work: open an issue.
- **Event updates** — new workshops, deadline changes, or discontinued series: PR to the events calendar.
- **Annual review input** — before each December review, nominate "paper of the year" candidates per category.

If you find this list useful, please also cite the survey:

```bibtex
@article{chen2025advancing,
    title = {Advancing Financial Engineering with Foundation Models: Progress, Applications, and Challenges},
    author = {Chen, Liyuan and Liu, Shuoling and Yan, Jiangpeng and Wang, Xiaoyu and Liu, Henglin and Li, Chuang and Jiao, Kecheng and Ying, Jixuan and Liu, Yang Veronica and Yang, Qiang and Li, Xiu},
    journal = {Engineering},
    year = {2025},
    doi = {10.1016/j.eng.2025.11.029},
    url = {https://doi.org/10.1016/j.eng.2025.11.029}
}
```
