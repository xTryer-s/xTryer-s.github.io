---
title: "MMMG: A Benchmark for Text-to-Image Reasoning"
excerpt: "A massive, multidisciplinary benchmark for evaluating multimodal reasoning in knowledge image generation across disciplines, educational levels, and visual formats.<br/><img src='/images/MMMG.png' style='width: 80%; max-width: 720px;'>"
collection: portfolio
---

## MMMG: A Massive, Multidisciplinary, Multi-Tier Generation Benchmark for Text-to-Image Reasoning  
Yuxuan Luo, Yuhui Yuan, Junwen Chen, **Haonan Cai**, Ziyi Yue, Yuwei Yang, Fatima Zohra Daha, Ji Li, Zhouhui Lian  

**Paper:** [arXiv:2506.10963](https://arxiv.org/abs/2506.10963)

### Overview
We introduce **knowledge image generation** as a new task to systematically evaluate the reasoning capability of modern text-to-image generation models. Knowledge images—such as diagrams, charts, and mind maps—play a fundamental role in human learning, as supported by **dual-coding theory** and the **picture-superiority effect**. Generating such images requires models to integrate **world knowledge**, **logical reasoning**, and **pixel-level grounding** into clear and explanatory visuals, posing challenges beyond conventional image synthesis.

To support comprehensive and controlled evaluation, we present **MMMG**, a **Massive, Multi-Discipline, Multi-Tier Knowledge-Image Generation Benchmark**.

### Benchmark Design
MMMG consists of **4,456 expert-validated knowledge image–prompt pairs**, covering:

- **10 disciplines** (e.g., science, humanities, engineering)
- **6 educational levels**, from elementary to professional
- **Diverse knowledge formats**, including charts, diagrams, and mind maps

To eliminate confounding visual complexity during evaluation, we adopt a **unified Knowledge Graph (KG) representation**, where each KG explicitly defines the target image’s core entities and their relational dependencies.

### Evaluation Protocol
We propose **MMMG-Score**, a dedicated metric for knowledge image generation that jointly measures:

- **Factual fidelity**, computed via graph-edit distance between predicted and ground-truth KGs
- **Visual clarity**, assessing the readability and organization of generated images

### Results
We conduct extensive evaluations on **16 state-of-the-art text-to-image models**, revealing substantial reasoning deficiencies, including low entity fidelity, weak relational modeling, and visual clutter. Notably, **GPT-4o achieves an MMMG-Score of only 50.20**, highlighting the benchmark’s difficulty.

To foster future research, we further release **FLUX-Reason**, an open and effective baseline that integrates a reasoning LLM with diffusion models and is trained on **16,000 curated knowledge image–prompt pairs**, achieving an MMMG-Score of **34.45**.

### Keywords
Text-to-Image Reasoning · Knowledge Image Generation · Multimodal Evaluation · Benchmark · Knowledge Graphs
