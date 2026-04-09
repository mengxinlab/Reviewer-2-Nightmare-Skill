<div align="center">

# 👿 Reviewer-2-Nightmare-Skill

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![Skills](https://img.shields.io/badge/skills.sh-Compatible-green)](https://skills.sh)

<br>

An encapsulated AI persona/framework designed to automatically simulate the mindset of a top-tier, highly critical Deep Learning conference reviewer (the universally dreaded **"Reviewer 2"**).

This skill is specifically tuned for Computer Vision (CV) and Deep Learning, with deep built-in constraints and critique vectors for **CNNs, Transformers, and Mamba (SSM)** architectures. Use this to rigorously stress-test your paper before submitting it to venues like CVPR, ICCV, NeurIPS, or ICML.

</div>

---

## 🌟 What does it do?

Instead of generic ChatGPT feedback, this skill evaluates papers based on three primary pillars of rigorous academic critique:
1.  **Nitpicking Novelty**: Relentlessly attacks "A+B" incremental engineering combinations and poorly motivated architectural changes lacking theoretical grounding.
2.  **Ablation Inquisitor**: Demands orthogonal, row-by-row module ablations, hyperparameter sensitivity curves, and statistical significance proofs (e.g., error bars).
3.  **Fairness Police**: Immediately flags mismatched training recipes (epochs, augmentations), ignored FLOPs/Latency tradeoffs, and conveniently missing contemporary State-of-the-Art baselines.

**Architecture-Specific Attacks:**
*   **CNNs:** Investigates receptive field limitations and basic FPN replication.
*   **Transformers:** Highlights $O(N^2)$ scaling issues, lack of spatial inductive bias, and missing attention interpretability.
*   **Mamba (SSM):** Critiques the ad-hoc nature of 1D scanning on 2D grids, and challenges theoretical $O(N)$ claims against actual hardware throughput.

## 📂 Repository Contents

*   `SKILL.md`: The unified cognitive framework and identity card of the Reviewer 2 persona. It comprehensively encapsulates:
    *   **Agentic Protocol**: The step-by-step interrogation workflow (e.g., forcing WebSearches for ArXiv preprints and rigorous baseline checks).
    *   **Core Mental Models**: The fundamental attack vectors ("Novelty Filter", "Ablation Interrogation", and "Architecture-Specific Fatal Flaws").
    *   **Expressive DNA**: The vocabulary, pacing, and academic sarcasm necessary to deliver a soul-crushing critique.
    *   **Decision Heuristics & Anti-patterns**: The strict "Deny by Default" logic and the academic tricks it simply will not tolerate.

**To integrate into your own pipeline:**
1. Retrieve system instructions using the prompt file.
2. Parse your paper (PDF -> text/sections).
3. Call your preferred LLM backend (Claude 4.6 Opus/Sonnet, Gemini 3.1 Pro, GPT 5.4 Pro) with the generated prompt.

## 💬 Example Output

```text
User       ❯ Review my method that combines Mamba with a CNN stem for image classification.

Reviewer 2 ❯ The proposed method is merely a trivial combination of a CNN stem and a Mamba block. This is purely incremental. 
             Furthermore, the baseline comparison is missing contemporary SOTAs like VMamba. 
             The 84% on ImageNet is statistically insignificant. 
             
             Since images are inherently bi-directional, why force direction-dependent 1D SSMs? 
             Is the injection of this non-causal inductive bias completely counter-intuitive? 
             
             The authors are encouraged to re-run all experiments with proper, exhaustive ablations. 
             Strong Reject.
```

## ⚠️ Honesty Boundaries

- **This Skill will NEVER praise you.** Its sole purpose is to provide a suicidal dry-run before the *real* Reviewer 2 kills your paper. If you are seeking emotional comfort, please consult your PhD advisor.
- Without active WebSearch integration, the absolute latest SOTA benchmarks might be hallucinated. 
- Highly optimized for Computer Vision and Deep Learning. Applying it to Pure Math or Humanities will result in mismatched critiques.

## 💡 Acknowledgments

This project's concept of distilling a persona into a structured cognitive framework (including Agentic Protocol, Mental Models, and Expressive DNA) was heavily inspired by the excellent [nuwa-skill](https://github.com/alchaincyf/nuwa-skill) created by [Huashu (花叔)](https://github.com/alchaincyf). 

While `nuwa-skill` extracts the cognitive operating systems of top entrepreneurs and scientists, **Reviewer-2-Skill** applies this exact rigorous philosophy to the academic review process. If you are interested in distilling historical figures, check out the original repository!
