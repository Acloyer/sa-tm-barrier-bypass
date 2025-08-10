# SA-TM

**Structurally-Aware Turing Machines (SA-TM): Oracle Model with Θ(log n) Introspection**

This repository contains the LaTeX source, bibliography, and supplementary material for a preprint that studies an **oracle** model of computation with bounded introspection and presents an **assumption-based oracle separation**.

---

## What this project claims (and what it does not)

**Claims (within the SA-TM oracle model):**
- **Model.** Deterministic **oracle** Turing machines with bounded-radius **Θ(log n)** introspection over code/state.
- **Main result.** Under standard complexity/crypto assumptions (**ETH**, **LWE**), we construct an oracle \(O\) such that  
  `P^O_SA != NP^O_SA` in the SA-TM model.
- **Barrier stance (model-dependent).** The proof strategy is designed to **avoid the templates** of the four classical barriers (relativization, natural proofs, algebrization, proof complexity) **within this oracle setting**, via non-black-box introspection and LWE-based pseudorandomness.

**Not claimed:**
- No non-oracle lower bounds for the **standard TM** model.
- No resolution of **P vs NP**.
- No global defeat of the four barriers **outside** the SA-TM oracle framework.

---

## Build (arXiv-safe; no shell-escape)

```bash
pdflatex main.tex
bibtex main     # if bibliography is used
pdflatex main.tex
pdflatex main.tex
