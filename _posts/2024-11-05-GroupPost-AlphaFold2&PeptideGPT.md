---
title: GroupPost20241105-AlphaFold2 & PeptideGPT
author: Bohao Lv
tags:
  - biology
  - medicine
  - generative-model
---

<!-- excerpt start -->
AF2, the champion of the 2021 CASP competition, is also the work that won the 2024 Nobel Prize and holds significant importance for protein engineering.

PeptideGPT is a pipeline to generate protein sequences with specific functions.

 <!-- excerpt end -->

The following is an overview of the presentations by Bohao Lv:

PeptideGPT：
- Finetuned the existing protein sequence generation model ProtGPT2 using protein data with specific functions to generate protein sequences with specific functions.
- Utilized bioinformatics knowledge to perform the first round of sequence rationality screening on the generated sequences.
- Used the structure prediction model ESMFold to perform the second round of rational structure screening on the generated sequences.
- Employed a classifier to validate the functions of the generated protein sequences.

AF2
- Decoder part
  -  IPA
  -  Backbone predict
  -  atom predict
- Loss function
 
The specific files can be found here: [AF2.pdf](https://github.com/AI3-GenAI4Sci/lab-website/blob/main/docs/AF2-20241119.pdf) & [PeptideGPT Blog](https://zhuanlan.zhihu.com/p/4412467760)
