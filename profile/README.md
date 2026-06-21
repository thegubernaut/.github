# Gubernaut Research

**The missing control layer for modern AI.**

We build the **Gubernaut Cognitive Controller (GCC)** — a deterministic,
model-agnostic control layer that wraps any LLM in a dual-process architecture
(a fast impulse layer, an executive arbiter, an episodic memory, a self-model)
under a homeostatic metacognitive controller. It does **not** retrain the host
model; it regulates it at runtime, and every regulatory decision is logged,
inspectable, and reproducible.

This is a control system, not a "mind" — no consciousness claims. The target is an
engineering objective: calm, evidence-responsive output under adversarial pressure.

### Validation — pre-registered, cross-family

Regulated output beats baseline in **15/16** generator×judge cells (11/12
off-diagonal, 4/4 diagonal) across four frontier model families, anchored on a
frozen three-model **8/9**. Generate-once / judge-many; the effect survives a
fully independent fourth judge family; every claim traces to logged, re-judgeable
runs (the one null cell is reported, unpatched).

- 📊 **Evidence & verification release:** [`gcc-validation`](https://github.com/thegubernaut/gcc-validation) — transcripts, judge panels (sha256), combined matrices, and the combine script. Recompute it yourself.
- 📄 White paper: forthcoming.

*Toronto.*
