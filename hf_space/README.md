---
title: Auctions with Risk Reserves for Scarce AI Research
emoji: ⚖️
colorFrom: green
colorTo: blue
sdk: static
app_file: index.html
pinned: false
short_description: Compare three rules for scarce AI research slots.
---

# FP08 — Auctions with Risk Reserves for Scarce AI Research

**Authors:** Zhenning Wang and Qianshuo (Aaron) Wang  
**Course:** COMSCI/ECON 206 — Computational Microeconomics, Autumn 2026

- [Live Hugging Face Space](https://huggingface.co/spaces/dku-comsci-econ206-2026/Final_Zhenning_Qianshuo_PM_Bid)
- [Root GitHub repository](https://github.com/AaronW-77/PS2_FP8_Qianshuo-Aaron-_Zhenning)

## Purpose and evidence status

This browser-only exploratory interface connects a synthetic allocation-mechanism
lab with a separate behavioral bidding task. The lab compares FCFS, pure
first-price auctions, and a hybrid risk reserve using N=20, K=4, R=1, r*=60,
and the stylized bid rule b=0.8v. This bid rule is not a multi-slot equilibrium.
The browser-generated batch is separate from the project's reported 1,000-batch
simulation; risk coverage is not demonstrated avoided financial loss.

The behavioral task is a **four-bidder, single-slot first-price auction**:
the highest bid wins and the winner pays their own bid. Under symmetric risk
neutrality and independent uniform private values, the Bayesian benchmark is
**b(v) = 3v/4**. Gain/loss framing uses identical numerical payoffs and differs
only in framing: winning yields v-b and losing yields zero. The self-play task
uses three computer opponents bidding 0.75v; Peer Play accepts four entered bids.
This task does not directly test Hybrid versus Pure.

**Behavioral evidence remains PLANNED.** The interface is an exploratory
behavioral artifact; no completed human-bidding experiment is reported as evidence
in the final project. The prefilled self/peer values and bids are illustrative
inputs, not collected observations. The aggregate evidence log starts empty;
any subsequently entered observations are descriptive and exploratory, not
population-level or causal evidence. Entries are held in the browser, with no
server-side storage or automatic submission. Do not enter sensitive information.

## Source synchronization

Copied from Hugging Face commit `f6b1ef435f1a9cde3978fa4c52f3bb000e7db896`
on 21 October 2026. `index.html` and `style.css` are byte-for-byte copies;
only this README is adapted for the GitHub source mirror. The original static
Space YAML configuration above is preserved. The live Space is not modified.

- `index.html`: complete interface, inline JavaScript, and active inline CSS.
- `style.css`: existing upstream stylesheet, preserved even though the current
  HTML does not link to it. Do not add a stylesheet link merely for this mirror;
  that would change the interface's appearance.

No separate JavaScript, package manifest, build step, API key, or external runtime
assets are required. Upstream's `.gitattributes` contains generic Git LFS rules,
not application source or runtime dependencies, and is not copied.

## Run locally

From the repository root, run `python3 -m http.server 8000`, then open
`http://localhost:8000/hf_space/`. Alternatively, open `hf_space/index.html`
directly in a browser. The interface is self-contained; outbound literature
links are navigation links rather than runtime dependencies.

To refresh this mirror, retrieve the actual files from the live Space repository,
copy the implementation files unchanged, review any file additions or removals,
and update the source commit recorded here. Keep the behavioral task distinct
from the main project's N=20/K=4 simulation and its reported results.
