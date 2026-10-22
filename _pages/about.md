---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a PhD student in theoretical chemistry at the University of Chicago, advised by [Aaron R. Dinner](https://dinner-group.uchicago.edu/) and [Jonathan Weare](https://cims.nyu.edu/~weare/).

My research develops generative and probabilistic sampling methods for molecular simulation and statistical physics. I am particularly interested in diffusion/flow-based molecular sampling, Gibbs sampling, posterior inference, and path-integral quantum statistics.

My recent work develops *generative Gibbs sampling*. A generative model is trained on statistics that are easy to sample, and an augmented Gibbs sampler then extends it to a much harder target by supplying the known physical structure at sampling time. The same trained model can therefore be reused across physical contexts without retraining.

[Download CV](/files/CV_Weizhou_Wang.pdf) / [Google Scholar](https://scholar.google.com/citations?user=OOckHoEAAAAJ&hl=en) / [GitHub](https://github.com/weizhouwangw) / [ORCID](https://orcid.org/0009-0004-6749-3003)

## Research Interests

- Generative models for molecular simulation
- Probabilistic sampling and posterior inference
- Statistical mechanics and path-integral methods
- Enhanced sampling and rare-event molecular dynamics
- Physics-aware AI for Science

## Selected Research

### Path-Integral Quantum Statistics from Classical Statistics

Imaginary-time path integrals capture nuclear quantum effects rigorously but are expensive to simulate. These two works recover quantum statistics using generative models trained only on classical simulation data and enable temperature transferability.

- **Quantum statistics from classical simulations via generative Gibbs sampling** (Generative Gibbs Sampling for Path Integrals, GG-PI). Learns the single-bead conditional density of the ring polymer from standard classical simulations and samples the path integral by Gibbs sampling. It transfers across temperatures without retraining and significantly reduces wall-clock time compared with path-integral molecular dynamics. [Paper](https://arxiv.org/abs/2601.20228) / [Code](https://github.com/weizhouwangw/GenerativeGibbsSamplingforPathIntegral) / [BibTeX](/files/wang2026ggpi.bib)
- **Nuclear quantum effects as a denoising problem** (DPI). Separates the quantum context from what is learned. A denoiser trained on classical Boltzmann statistics alone is composed at sampling time with an analytic Gaussian step that carries the quantum context. The same denoiser transfers exactly across temperature, isotopic mass, dissipation strength, and path boundary conditions, including open paths that give momentum distributions. [Paper](https://arxiv.org/abs/2607.19680)

### Composing Diffusion Priors with Physical Context

Pretrained diffusion models are powerful priors, but a scientific target often depends on physical context, such as solvent, ions, or interacting molecules, that no single model represents.

- **Composing diffusion priors with explicit physical context via generative Gibbs sampling** (Generative Gibbs for Physics-Aware Sampling, GG-PA), *NeurIPS 2026*. A training-free framework that treats learned partial priors and explicit physical context as one joint target in an augmented space. Its Gibbs sampler is asymptotically exact as the diffusion time goes to zero and stays exact at finite diffusion time for quadratic interactions, the case that DPI realizes for path integrals. It recovers context-induced distribution shifts and emergent collective behavior, from a φ⁴ lattice model to atomistic peptide systems, without retraining. [Paper](https://arxiv.org/abs/2605.10642) / [Code](https://github.com/weizhouwangw/GG-PA) / [Talk](https://www.microsoft.com/en-us/research/video/generative-gibbs-sampling-composing-generative-models-with-explicit-physical-context/) / [BibTeX](/files/wang2026ggpa.bib)

## News

- **Sep 2026** · GG-PA (Generative Gibbs for Physics-Aware Sampling) accepted at NeurIPS 2026.
- **Sep 2026** · Talk on generative Gibbs sampling at the [Microsoft Research New England Generative Modeling & Sampling Seminar](https://www.microsoft.com/en-us/research/event/microsoft-research-new-england-generative-modeling-sampling-seminar/) ([video](https://www.microsoft.com/en-us/research/video/generative-gibbs-sampling-composing-generative-models-with-explicit-physical-context/)).
- **Aug 2026** · Oral presentation on GG-PI and poster on GG-PA at [ACS Fall 2026](https://www.acs.org/events/all-events/acs-fall-2026.html), Chicago.
- **Jul 2026** · Runner-up for the Best Contributed Talk Award at PIQM 2026, Fudan University, Shanghai.
- **May 2026** · Awarded the Josef Fried Graduate Fellowship by the Department of Chemistry, University of Chicago.

## Honors and Fellowships

- **Best Contributed Talk Award, Runner-up**, CECAM Flagship School on Path Integral Quantum Mechanics in the Era of Machine Learning (PIQM 2026), Fudan University, 2026.
- **Josef Fried Graduate Fellowship**, Department of Chemistry, University of Chicago, 2026-2027. Awarded in recognition of excellence in research.
- **[Neubauer Family Distinguished Doctoral Fellow](https://grad.uchicago.edu/fellowships/neubauer-fellows/)**, University of Chicago, 2024-present.
