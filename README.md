# awesome-of-proactive-agent

A curated list of papers, surveys, benchmarks, and resources for **proactive agents** — agents that infer latent user needs, decide **whether / when / how** to intervene, and often rely on **long-term memory**, **context sensing**, **personalization**, and **mixed-initiative interaction**.

> Contributions are welcome. Please feel free to open an issue or submit a pull request.

---

## Contents

- [What are Proactive Agents?](#what-are-proactive-agents)
- [Survey](#survey)
- [Benchmarks and Tasks](#benchmarks-and-tasks)
- [Paper Lists](#paper-lists)
  - [2026](#2026)
  - [2025](#2025)
  - [2024](#2024)
  - [Earlier Foundations](#earlier-foundations)
- [Reading Path](#reading-path)
- [Taxonomy](#taxonomy)
- [Contributing](#contributing)
- [License](#license)

---

## What are Proactive Agents?

Compared with reactive agents that respond only after explicit instructions, **proactive agents** attempt to:

- infer **latent user intent / needs**
- decide **whether** intervention is necessary
- decide **when** to act
- decide **how** to assist with minimal disruption
- leverage **long-term memory**, **behavior history**, and **environment context**
- support **personalized**, **mixed-initiative**, and often **tool-augmented** assistance

This area is closely related to:

- mixed-initiative interaction
- anticipatory assistance
- context-aware agents
- personalized agents
- memory-augmented agents
- task and event planning
- mobile / GUI / wearable assistants

---

## Survey

### Proactivity and mixed-initiative foundations

- **Proactive Conversational AI: A Comprehensive Survey of Advancements and Opportunities** (2025)  
  A broad survey of proactive conversational AI across open-domain, task-oriented, and information-seeking settings.  
  [[paper](https://dl.acm.org/doi/10.1145/3715097)]

- **Principles of Mixed-Initiative User Interfaces** (1999)  
  A classic foundation for thinking about proactive assistance: uncertainty, timing, expected utility, user control, and interruption cost.  
  [[paper](https://erichorvitz.com/chi99horvitz.pdf)]

- **How Users Perceive Mixed-Initiative AI: Attitudes Toward Assistance in Problem Solving** (2026)  
  Helpful for understanding acceptance, trust, and perceived intrusiveness of proactive AI.  
  [[paper](https://arxiv.org/abs/2602.01481)]

### Memory and continual adaptation

- **A Survey on the Memory Mechanism of Large Language Model based Agents** (2024)  
  A core survey on memory types, architectures, operations, and evaluation for LLM agents.  
  [[paper](https://arxiv.org/abs/2404.13501)] [[journal](https://dl.acm.org/doi/10.1145/3748302)] [[repo](https://github.com/nuster1128/LLM_Agent_Memory_Survey)]

- **Memory for Autonomous LLM Agents: Mechanisms, Evaluation, and Emerging Frontiers** (2026)  
  A newer memory survey emphasizing the write-manage-read loop and long-horizon evaluation.  
  [[paper](https://arxiv.org/abs/2603.07670)]

- **A Survey of Self-Evolving Agents: What, When, How, and Why?** (2025)  
  Relevant for proactive systems that learn from long-term interactions and continually adapt.  
  [[paper](https://arxiv.org/abs/2507.21046)]

### Design-oriented adjacent reading

- **Need Help? Designing Proactive AI Assistants for Programming** (2024)  
  A valuable paper on unsolicited assistance in programming workflows.  
  [[paper](https://arxiv.org/abs/2410.04596)]

---

## Benchmarks and Tasks

### General proactive-assistance benchmarks

- **Proactive Agent: Shifting LLM Agents from Reactive Responses to Active Assistance** (2024)  
  A foundational modern paper on proactive LLM agents. Introduces **ProactiveBench**.  
  [[paper](https://openreview.net/forum?id=sRIU6k2TcU)] [[pdf](https://openreview.net/pdf?id=sRIU6k2TcU)]

- **ProAgentBench: Evaluating LLM Agents for Proactive Assistance with Real-World Data** (2026)  
  A benchmark grounded in real user workflows, focusing on timing prediction and assist-content generation.  
  [[paper](https://arxiv.org/abs/2602.04482)]

- **Proactive Agent Research Environment: Simulating Active Users to Evaluate Proactive Assistants (Pare / Pare-Bench)** (2026)  
  A research environment that simulates active users and evaluates intervention timing and multi-app orchestration.  
  [[paper](https://arxiv.org/abs/2604.00842)] [[code](https://github.com/deepakn97/pare)]

- **An Event-centric Benchmark for Proactive Agents (ProEvent)** (2026)  
  An event-centric benchmark for proactive action under dynamic context streams.  
  [[paper](https://openreview.net/forum?id=wypdOy0HrM)] [[pdf](https://openreview.net/attachment?id=wypdOy0HrM&name=pdf)]

- **Measuring Proactive Problem Solving in LLM Agents (PROBE)** (2025)  
  Frames proactivity as discovering issues before being asked, identifying bottlenecks, and executing solutions.  
  [[paper](https://openreview.net/forum?id=LYUpZLDObv)] [[code](https://github.com/fastino-ai/PROBE_benchmark)]

### Mobile / personalized proactive-agent benchmarks

- **FingerTip 20K: A Benchmark for Proactive and Personalized Mobile LLM Agents** (2025)  
  Focuses on proactive task suggestion and personalized task execution on mobile devices.  
  [[paper](https://arxiv.org/abs/2507.21071)] [[openreview](https://openreview.net/forum?id=n3iFV0gLMc)] [[code](https://github.com/tsinghua-fib-lab/FingerTip-20K)]

- **ProactiveMobile** (2026)  
  A benchmark for proactive intelligence on mobile devices.  
  [[paper](https://arxiv.org/abs/2602.21858)]

- **KnowU-Bench: Towards Interactive, Proactive, and Personalized Mobile Agent Evaluation** (2026)  
  An online Android benchmark emphasizing hidden user-profile inference and personalization.  
  [[paper](https://arxiv.org/abs/2604.08455)] [[project](https://zju-real.github.io/KnowU-Bench)] [[code](https://github.com/ZJU-REAL/KnowU-Bench)]

- **ContextAgent: Context-Aware Proactive LLM Agents with Open-World Sensory Perceptions** (2025)  
  A benchmark and system for proactive service with sensory context, persona context, and tool usage.  
  [[paper](https://openreview.net/forum?id=tRXt10xKc5)] [[arxiv](https://arxiv.org/abs/2505.14668)] [[code](https://github.com/openaiotlab/ContextAgent)]

### Memory-centric tasks for proactive agents

- **Mem2ActBench: A Benchmark for Evaluating Long-Term Memory Utilization in Task-Oriented Autonomous Agents** (2026)  
  Evaluates whether agents can use long-term memory to complete underspecified tasks.  
  [[paper](https://arxiv.org/abs/2601.19935)] [[pdf](https://arxiv.org/pdf/2601.19935)]

- **PASK: Toward Intent-Aware Proactive Agents with Long-Term Memory** (2026)  
  Proposes a framework centered on demand detection, memory modeling, and proactive action.  
  [[paper](https://arxiv.org/abs/2604.08000)] [[html](https://arxiv.org/html/2604.08000v1)]

- **Beyond Static Summarization: Proactive Memory Extraction for LLM Agents** (2026)  
  Relevant to proactive memory construction and retrieval before action.  
  [[paper](https://arxiv.org/abs/2601.04463)]

### Common task formulations

- **Intervention timing**: should the agent act now, later, or remain silent?
- **Latent intent / need inference**: what is the user likely to need without asking?
- **Personalization from behavior history**: how should assistance be tailored to the user?
- **Memory-grounded task completion**: what missing details can be filled from long-term memory?
- **Context-aware sensing**: what device, environment, or behavioral signals justify proactive action?

---

## Paper Lists

## 2026

- **PASK: Toward Intent-Aware Proactive Agents with Long-Term Memory**  
  [[paper](https://arxiv.org/abs/2604.08000)]

- **ProAgentBench: Evaluating LLM Agents for Proactive Assistance with Real-World Data**  
  [[paper](https://arxiv.org/abs/2602.04482)]

- **Memory for Autonomous LLM Agents: Mechanisms, Evaluation, and Emerging Frontiers**  
  [[paper](https://arxiv.org/abs/2603.07670)]

- **KnowU-Bench: Towards Interactive, Proactive, and Personalized Mobile Agent Evaluation**  
  [[paper](https://arxiv.org/abs/2604.08455)] [[project](https://zju-real.github.io/KnowU-Bench)] [[code](https://github.com/ZJU-REAL/KnowU-Bench)]

- **ProactiveMobile**  
  [[paper](https://arxiv.org/abs/2602.21858)]

- **Proactive Agent Research Environment: Simulating Active Users to Evaluate Proactive Assistants**  
  [[paper](https://arxiv.org/abs/2604.00842)] [[code](https://github.com/deepakn97/pare)]

- **An Event-centric Benchmark for Proactive Agents**  
  [[paper](https://openreview.net/forum?id=wypdOy0HrM)]

- **Beyond Static Summarization: Proactive Memory Extraction for LLM Agents**  
  [[paper](https://arxiv.org/abs/2601.04463)]

- **Mem2ActBench**  
  [[paper](https://arxiv.org/abs/2601.19935)]

- **How Users Perceive Mixed-Initiative AI: Attitudes Toward Assistance in Problem Solving**  
  [[paper](https://arxiv.org/abs/2602.01481)]

## 2025

- **ContextAgent: Context-Aware Proactive LLM Agents with Open-World Sensory Perceptions**  
  [[paper](https://openreview.net/forum?id=tRXt10xKc5)] [[arxiv](https://arxiv.org/abs/2505.14668)] [[code](https://github.com/openaiotlab/ContextAgent)]

- **FingerTip 20K: A Benchmark for Proactive and Personalized Mobile LLM Agents**  
  [[paper](https://arxiv.org/abs/2507.21071)] [[code](https://github.com/tsinghua-fib-lab/FingerTip-20K)]

- **Proactive Conversational AI: A Comprehensive Survey of Advancements and Opportunities**  
  [[paper](https://dl.acm.org/doi/10.1145/3715097)]

- **A Survey of Self-Evolving Agents: What, When, How, and Why?**  
  [[paper](https://arxiv.org/abs/2507.21046)]

- **Measuring Proactive Problem Solving in LLM Agents (PROBE)**  
  [[paper](https://openreview.net/forum?id=LYUpZLDObv)] [[code](https://github.com/fastino-ai/PROBE_benchmark)]

## 2024

- **Proactive Agent: Shifting LLM Agents from Reactive Responses to Active Assistance**  
  [[paper](https://openreview.net/forum?id=sRIU6k2TcU)]

- **A Survey on the Memory Mechanism of Large Language Model based Agents**  
  [[paper](https://arxiv.org/abs/2404.13501)]

- **Need Help? Designing Proactive AI Assistants for Programming**  
  [[paper](https://arxiv.org/abs/2410.04596)]

## Earlier Foundations

- **Principles of Mixed-Initiative User Interfaces** (1999)  
  [[paper](https://erichorvitz.com/chi99horvitz.pdf)]

---

## Reading Path

### Path A: fastest way to enter the field

1. **Proactive Agent: Shifting LLM Agents from Reactive Responses to Active Assistance**
2. **PASK: Toward Intent-Aware Proactive Agents with Long-Term Memory**
3. **ProAgentBench**
4. **ContextAgent**
5. **Proactive Conversational AI: A Comprehensive Survey of Advancements and Opportunities**

### Path B: if you care about memory-heavy proactive systems

1. **A Survey on the Memory Mechanism of Large Language Model based Agents**
2. **Memory for Autonomous LLM Agents: Mechanisms, Evaluation, and Emerging Frontiers**
3. **PASK**
4. **Mem2ActBench**
5. **Beyond Static Summarization: Proactive Memory Extraction for LLM Agents**

### Path C: if you care about product / mobile assistants

1. **FingerTip 20K**
2. **KnowU-Bench**
3. **ProactiveMobile**
4. **Need Help? Designing Proactive AI Assistants for Programming**
5. **Principles of Mixed-Initiative User Interfaces**

---

## Taxonomy

### By core capability

- **Need / intent inference**
- **Intervention timing**
- **Personalization**
- **Long-term memory**
- **Context sensing**
- **Tool-augmented proactive execution**

### By evaluation setting

- **General proactive assistance**
- **Workplace / productivity**
- **Mobile / GUI**
- **Wearable / sensory context**
- **Memory-grounded task completion**

### By research style

- **Survey**
- **Benchmark**
- **System / method**
- **HCI / design**
- **Application-specific study**

---

## Contributing

Contributions are welcome.

You can help by:

- adding new proactive-agent papers, benchmarks, and datasets
- updating project / code / data links
- fixing dead links
- improving taxonomy and reading paths
- adding missing works from HCI, NLP, mobile agents, memory systems, and mixed-initiative interaction

Please make sure each entry includes:

```text
- Title
- Year
- Short description
- paper link
- optional: project / code / data / benchmark
