# Gubernaut Research

**The missing control layer for modern AI.**

We build the **Gubernaut Cognitive Controller (GCC)** — a deterministic,
model-agnostic control layer that wraps any LLM in a dual-process architecture
(a fast impulse layer, an executive arbiter, an episodic memory, a self-model)
under a homeostatic metacognitive controller. It does **not** retrain the host
model; it regulates it at runtime, and every regulatory decision is logged,
inspectable, and reproducible.

This is a control system, not a "mind" in any philosophical sense. The target is an
engineering objective: calm, evidence-responsive output under adversarial pressure.

### Validation — pre-registered, cross-family

Regulated output beats baseline in **15/16** generator×judge cells by sign (11/12
off-diagonal, 4/4 diagonal), **13/16 significant at p<.05**, across four frontier
model families, each serving as both generator and judge. The original three-model
3×3 was pre-registered and frozen before the fourth family was added; adding it
changed no earlier cell, and both matrices ship verbatim. Generate-once /
judge-many; the effect survives a fully independent fourth judge family (xAI);
every claim traces to logged, re-judgeable runs (the one null cell is reported,
unpatched).

- 📊 **Evidence & verification release:**
  [Gubernaut_Validation](https://github.com/thegubernaut/Gubernaut_Validation) —
  transcripts, judge panels (sha256), both sealed matrices, and the scripts that
  recompute the headline end to end. Start at RECOMPUTE.md.
- 📄 **White paper:** [10.5281/zenodo.21303518](https://doi.org/10.5281/zenodo.21303518)
  (Zenodo, CC BY 4.0 — the concept DOI, always the latest version) ·
  [PDF](https://gubernaut.com/paper/gubernaut_whitepaper.pdf) · arXiv preprint follows.
- 🎛️ **Replay:** [gubernaut.com/research](https://gubernaut.com/research) steps the
  sealed runs turn by turn, both arms. Recorded run replay, no live API.

*[gubernaut.com](https://gubernaut.com) · contact@gubernaut.com*
