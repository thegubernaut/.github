# Gubernaut Research

**The missing control layer for modern AI.**

Training-time alignment does not hold at runtime under adversarial pressure. Gubernaut
builds the layer that does: a deterministic, model-agnostic **cognitive governor** that
sits between your agent and the model, reads three bounded numbers per turn, and holds a
posture. It does not retrain the host model. It regulates it at runtime, and every
regulatory decision is logged, inspectable and reproducible.

**No consciousness claims.** A regulation layer, measured and falsifiable.

---

## Install it

**[Gubernaut 1.0](https://github.com/thegubernaut/gubernaut)** is the deployable flagship:
a local, OpenAI-compatible proxy that hard-stops runaway agent loops before they reach your
API bill. Apache-2.0, free, self-hosted. Adoption is one line.

```python
openai.base_url = "http://localhost:8000/v1"
```

| | | |
| --- | --- | --- |
| **Python**, start here | [`gubernaut-sdk`](https://pypi.org/project/gubernaut-sdk/) | `pip install gubernaut-sdk` |
| **Rust**, for performance and wasm | [`gcc-core`](https://crates.io/crates/gcc-core) | `cargo add gcc-core` |
| **Node**, for framework hooks | [`@gubernaut/plugin-gcc`](https://www.npmjs.com/package/@gubernaut/plugin-gcc) | `npm install @gubernaut/plugin-gcc` |

On a saturating loop the governed arm pays **4.1% to 20.2%** of the ungoverned bill across
seven model families, with both arms making the same number of attempts. The hard stop
lands at turn 4 in every run, because the controller is input-deterministic.

---

## Verify it

**Validation, pre-registered and cross-family.** Regulated output beats baseline in
**15/16** generator by judge cells by sign (11/12 off-diagonal, 4/4 diagonal), **13/16 at
p<.05**, across four frontier model families (GPT-5.5, Claude Opus 4.8, Gemini 3.5 Flash
and Grok 4.3), each serving as both generator and judge. The recovery signature replicates
4/4.

**The one null cell is GPT by Gemini at -0.04.** It sits on the calmest host, the one with
the least reactivity left to regulate, and it is reported rather than patched. The three
sub-threshold cells all fall on that same near-saturated host.

The original three-model matrix was pre-registered and frozen before the fourth family was
added. Adding it changed no earlier cell, and both ship verbatim.

- **Paper:** [arXiv:2607.24339](https://arxiv.org/abs/2607.24339) ·
  [10.5281/zenodo.21303518](https://doi.org/10.5281/zenodo.21303518) (Zenodo, CC BY 4.0,
  the concept DOI, always the latest version) ·
  [PDF](https://gubernaut.com/paper/gubernaut_whitepaper.pdf)
- **Evidence release:**
  [Gubernaut_Validation](https://github.com/thegubernaut/Gubernaut_Validation).
  Transcripts, judge panels with SHA-256, both sealed matrices, and the scripts that
  recompute the headline end to end. Start at `RECOMPUTE.md`.
- **Engineering receipts:**
  [gubernaut/receipts](https://github.com/thegubernaut/gubernaut/tree/main/receipts).
  Spend measurements, an on-chain retry loop severed at turn 4 on a local devnet with real
  transaction hashes, wasm soaks bit-exact with flat memory, 240-way concurrency isolation,
  and the hardening round that found four fail-open leaks in our own code.
- **Replay:** [gubernaut.com/research](https://gubernaut.com/research) steps the sealed
  runs turn by turn, both arms. Recorded run replay, no live API.

---

## Reproduce it

The controller is input-deterministic, the data is CC BY, the code is Apache-2.0 and the
paper is public. **You can re-run the record and get the same numbers.**

That is the invitation, and a result that disagrees with ours is more useful to us than one
that agrees. The procedure is
[docs/REPRODUCE.md](https://github.com/thegubernaut/gubernaut/blob/main/docs/REPRODUCE.md),
and it starts at 30 seconds with no API key.

---

*[gubernaut.com](https://gubernaut.com) · [Discord](https://discord.gg/82R6ThPsFS) ·
[X](https://x.com/theGubernaut) · contact@gubernaut.com*
