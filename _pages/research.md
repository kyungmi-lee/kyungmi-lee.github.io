---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

<div class="notice notice--large" markdown="1">
:star2: **[Prospective Students]** If you are looking for a Ph.D. advisor and if the research questions below excite you, please feel free to drop me an email with your CV.
</div>

## Current Interests

### Trustworthy Computing for AI
As AI applications handle private information and influence our decision-making, we want them to be trustworthy - protecting our information, preserving integrity, and being available when we need them. 
My research vision is that this trust should be rooted and supported by the hardware, which is at the foundation of AI systems. 
Some of the questions that currently motivate my research include:
- How do we *limit or scale* the trusted computing base for accelerator-rich computing systems?
- How do we scale critical *cryptographic primitives* for trustworthy AI computing?
- How can we achieve *synergy* between analog solutions and digital solutions for efficient security? 

### Projecting the Future of AI Hardware
AI hardware is an exciting research area where both the workloads and the underlying semiconductor technologies evolve rapidly. 
To shape the future of AI computing in a principled manner, we need characterization and modeling of these workloads and technologies. 
My research seeks to answer questions such as:
- What are the performance and energy bottlenecks of *evolving AI workloads*?
- What abstractions and architectural changes are needed to leverage *emerging circuit technologies*?

---

## Previous Work

### Secure AI Hardware

Hardware support for memory encryption and authentication for AI accelerators:
- **SecureLoop** ([MICRO'23](https://dl.acm.org/doi/10.1145/3613424.3614273)): Illustrates how cryptographic operations add constraints to the mapping of AI accelerators, and develops a design space exploration framework to determine the optimal mapping of workloads and systematically compare various architectural decisions. 
- **Sorbet** ([TVLSI'26](https://ieeexplore.ieee.org/document/11343916)): Realizes a secure AI accelerator with full memory encryption and authentication in 28nm CMOS, with modest overhead even for resource-constrained edge accelerators. 

Faults, side-channels, and adversarial attacks:
- **SparseBFA** ([ICASSP'22](https://ieeexplore.ieee.org/document/9747337)): Demonstrates that even a handful of bit flips in sparse matrix formats representing neural network parameters result in severe accuracy degradation
- Other works and collaborations include a lightweight fault detection mechanism for AI accelerators, implemented in 28nm CMOS ([ESSCIRC'23](https://ieeexplore.ieee.org/document/10268746), [JSSC'24](https://ieeexplore.ieee.org/document/10476588)), a novel side-channel in sparse accelerators that allows adversaries to learn input-dependent sparsity patterns ([CAL'24](https://ieeexplore.ieee.org/document/10521735)), and a characterization of robustness-efficiency trade-off of AI models on edge GPUs ([SiPS'21](https://ieeexplore.ieee.org/document/9604923), [OJCAS'21](https://ieeexplore.ieee.org/document/9645046)). 

An overview of security for AI hardware and my line of work in this topic is summarized in our review paper ([MCAS'25](https://ieeexplore.ieee.org/document/10876846)).

### Understanding Performance and Energy Consumption of GPUs

Estimating how much energy GPUs consume when they process AI workloads:
- **EnergAIzer** ([ISPASS'26](https://ieeexplore.ieee.org/document/11527276)): Provides a fast and accurate GPU power estimation framework for AI workloads, reducing the wall-time for estimation from hours to a few seconds, and enables power-aware design explorations of AI models, frequency-voltage settings, etc. 
- More work on multi-GPU LLM serving (pre-print [here](https://arxiv.org/abs/2605.14249)) and KV cache offloading coming soon

--- 

## Side Note

I'm also interested in the emerging intersection of AI and hardware design itself. 
For example, can agentic AI architect domain-specific accelerators for novel, not well-understood applications? 
How can we gauge the capability of agentic AI for hardware design and explain why it is good or bad at doing certain design tasks? 
I'd welcome any ideas on these open-ended questions.