---
title: GroupPost20240304-COT Compress
author: Rui Xu
tags:
  - LLM
  - reinforce-learning
  - COT
---

<!-- excerpt start -->

**Report Overview**

This report explores Chain-of-Thought (COT) compression techniques aimed at reducing the computational cost and enhancing the efficiency of large language models (LLMs) in complex reasoning tasks. While COT improves LLM performance by generating intermediate reasoning steps, the length of these reasoning chains leads to increased computational demands. COT compression seeks to shorten these chains without significantly impacting model performance.
 
 <!-- excerpt end -->

**Key Strategies and Methods**

The report covers several key strategies for COT compression:

1.  **Explicit Compression During Training:**
    *   **Knowledge Distillation:** This involves transferring knowledge from a complex "System 2" model (which generates COT) to a more efficient "System 1" model (which directly outputs results), thereby speeding up the inference process.
        * Notable work: Meta's "Distilling System 2 into System 1."
    *   **Step-by-Step Training:** This method iteratively trains models to identify and skip redundant reasoning steps, effectively shortening the reasoning pathway.
        * Notable work: Research by Qiu et al. in "Can Language Models Learn to Skip Steps?".
    *   **Data-Conditioned Training:** Utilizes GPT-4 to create pairs of long and short COT data, training models to generate reasoning chains of varying lengths.
        * Notable work: Research by BeiKe, "C3OT: Generating Shorter Chain-of-Thought without Compromising Effectiveness."
2.  **Hidden State Compression:**
    *   **Implicit COT:** Gradually internalizes the explicit COT reasoning process into the model's hidden states, eliminating the need for explicit reasoning chains.
        * Notable work: Research by Yejin Choi et al., "From Explicit CoT to Implicit CoT: Learning to Internalize CoT Step by Step."
    *   **Compressed COT (CCOT):** Employs densely semantic tokens to represent compressed reasoning, compressing reasoning chains within the hidden space.
        * Notable work: Research by JHU, "Compressed Chain of Thought: Efficient Reasoning Through Dense Representations."
3.  **Dynamic Length Control:**
    *   **COT-Valve:** Introduces adjustable parameters within the model's parameter space to dynamically manage the length of reasoning chains.
        * Notable work: Research by NUS, "COT-Valve: Length-Compressible Chain-of-Thought Tuning."
4.  **Reinforcement Learning Compression:**
    *   **O1-Pruner:** Designs a length-harmonizing reward function to guide models in generating shorter yet accurate reasoning sequences through reinforcement learning.
        * Notable work: Research by Sun Yat-sen University, "O1-Pruner: Length-Harmonizing Fine-Tuning for O1-Like Reasoning Pruning."
    *   **Kimi k1.5:** Explores various reinforcement learning compression strategies, including model merging, shortest rejection sampling, DPO, and Long2short RL.
        * Notable work: Kimi 1.5 Technical Report.

**Key Research Trends**

* A shift from explicit token compression to implicit representation compression, focusing on more efficient reasoning methods.
* The growing prominence of reinforcement learning in reasoning chain compression.
* The exploration of multi-agent frameworks for social reasoning.

**Future Outlook**

* As models continue to scale, managing inference costs will become increasingly critical.
* The development of more effective compression techniques is essential for deploying LLMs in resource-constrained environments.

**Report Significance**

* Provides a comprehensive overview of COT compression technologies, highlighting the latest advancements in the field.
* Offers practical insights for optimizing LLM performance and efficiency through appropriate compression strategies.
 
The specific files can be found here: [Trend Report.pdf](https://github.com/AI3-GenAI4Sci/lab-website/blob/main/docs/Trend_Report_of_Chain_Compression_in_reasoning_model.pdf)
