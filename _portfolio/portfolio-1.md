---
title: "Beyond Patches: Global-aware Autoregressive Font Generation"
excerpt: "A global-aware autoregressive framework for multimodal few-shot font generation, enabling coherent structure and flexible language-guided style control.<br/><img src='/images/GAR_Font.jpg' style='width: 80%; max-width: 380px;'>"
collection: portfolio
---

## Beyond Patches: Global-aware Autoregressive Model for Multimodal Few-Shot Font Generation  
**Haonan Cai**, Yuxuan Luo, Zhouhui Lian  

**Paper:** [arXiv:2601.01593](https://arxiv.org/abs/2601.01593)

### Overview
Manual font design requires translating an abstract stylistic concept into a complete and coherent glyph set, a process that is both time-consuming and expertise-intensive. This challenge is further amplified in **Few-shot Font Generation (FFG)**, where only a handful of reference glyphs are available. Existing methods often struggle to simultaneously preserve **global stylistic consistency** and **local structural correctness**, especially under limited supervision.

While **autoregressive (AR) models** have shown strong generative capabilities, their application to FFG is hindered by conventional **patch-level tokenization**, which fails to capture global font-level dependencies. Moreover, most prior approaches remain confined to an **image-to-image paradigm**, ignoring the expressive power of **language** in conveying font design intent.

### Method
We propose **GAR-Font**, a novel **global-aware autoregressive framework** for multimodal few-shot font generation. The key components include:

- **Global-aware Tokenizer**  
  Captures both fine-grained local structures and long-range global stylistic patterns, overcoming the limitations of patch-based representations.

- **Multimodal Style Encoder**  
  Enables flexible style control via a lightweight **language-style adapter**, allowing textual descriptions to guide font generation **without expensive multimodal pretraining**.

- **Post-refinement Pipeline**  
  Further improves structural fidelity and stylistic coherence, producing cleaner and more visually consistent glyphs.

### Results
Extensive experiments demonstrate that **GAR-Font consistently outperforms existing FFG methods**, achieving:
- Superior **global style faithfulness**
- Improved **structural integrity**
- High-quality generation with **textual stylistic guidance**

These results highlight the effectiveness of integrating global-aware modeling and multimodal control into autoregressive font generation.

### Keywords
Few-shot Font Generation · Autoregressive Models · Multimodal Learning · Global Representation · Image Synthesis
