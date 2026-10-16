### Taishi Namba

Independent researcher in theoretical physics (Atsugi, Japan).
I work on the foundations of statistical mechanics and on testable models of
gravity-related decoherence, and I am interested in where these ideas meet
machine learning.

[![ORCID](https://img.shields.io/badge/ORCID-0009--0002--7098--970X-A6CE39?logo=orcid&logoColor=white)](https://orcid.org/0009-0002-7098-970X)

**How I work.** Every analytical result in my papers is checked by code that
anyone can run. Each repository below has automated verification (GitHub
Actions) and an archived version with a DOI.

---

#### Papers and verification code

| Paper | Preprint | Code | Checks |
|---|---|---|---|
| *Can a learned score see the margin of the arrow of time?* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23408213.svg)](https://doi.org/10.5281/zenodo.23408213) | [learned-score-arrow-of-time](https://github.com/neginyan/learned-score-arrow-of-time) | 68 |
| *The resolution gap in many degrees of freedom* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23371932.svg)](https://doi.org/10.5281/zenodo.23371932) | [resolution-gap-many-dof](https://github.com/neginyan/resolution-gap-many-dof) | 543 |
| *A resolution gap for the coarse-grained arrow of time in nonlinear Hamiltonian flows* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23320603.svg)](https://doi.org/10.5281/zenodo.23320603) | [resolution-gap-arrow-of-time](https://github.com/neginyan/resolution-gap-arrow-of-time) | 336 |
| *A stretching-rate threshold for phase-space diffusion models with isotropic marginal noise schedules* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23181225.svg)](https://doi.org/10.5281/zenodo.23181225) | [phase-space-diffusion-threshold](https://github.com/neginyan/phase-space-diffusion-threshold) | 113 |
| *Sharp criterion for the coarse-grained arrow of time in Hamiltonian dynamics* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23258135.svg)](https://doi.org/10.5281/zenodo.23258135) | [coarse-grained-arrow-of-time](https://github.com/neginyan/coarse-grained-arrow-of-time) | 33 |
| *Causal consistency of Diósi–Penrose reduction and a profile-independent mass scale M_P/√2* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23064513.svg)](https://doi.org/10.5281/zenodo.23064513) | [causal-consistency-dp-reduction](https://github.com/neginyan/causal-consistency-dp-reduction) | 55 |
| *The spacetime carrier substrate: bandlimited information, regular geometry, and a gravitational Heisenberg cut* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22976896.svg)](https://doi.org/10.5281/zenodo.22976896) | [spacetime-carrier-substrate](https://github.com/neginyan/spacetime-carrier-substrate) | 117 |

#### Try it in your browser

Three short notebooks reproduce a central result each in a minute or two on a CPU (Google Colab, no installation):

- **The arrow of time through a blurry lens.** Pendulums on their unstable top: with the blur fixed the coarse-grained entropy falls; blurring slightly slower than the stretching rate is still enough, because a finite resolution leaves a margin.
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neginyan/resolution-gap-arrow-of-time/blob/main/demo/arrow_of_time_demo.ipynb)
- **Sampling below the threshold.** A phase-space diffusion model sampled with the exact score: below the threshold the clipped reverse SDE shrinks every mode, the corrected sampler does not.
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neginyan/phase-space-diffusion-threshold/blob/main/demo/sampler_below_threshold.ipynb)
- **Many degrees of freedom, checked blind.** A search over all Gaussian states of two coupled pendulums, from random starts, lands on the matrix formula; widening along a momentum costs nothing; the sealed predictions are downloaded, hash-checked and recomputed.
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neginyan/resolution-gap-many-dof/blob/main/demo/resolution_gap_many_dof.ipynb)

#### In one line each

- **Learned scores.** Small networks trained by denoising score matching read
  the arrow-of-time margin to within 2 % in two and four dimensions; a
  stochastic equation with the physical drift needs noise at least as fast as
  the stretching, while the entropy keeps growing in a band below it.
- **Many degrees of freedom.** One matrix formula gives the resolution gap of
  the best Gaussian state in any number of degrees of freedom: momentum
  directions and uncoupled modes cost nothing, and six predictions sealed
  before computing were confirmed.
- **Resolution gap.** For nonlinear flows the arrow-of-time criterion is proved
  for every Gaussian state; at finite resolution σ the threshold is missed by a
  margin proportional to σ (exact for the pendulum, observed for mixtures).
- **Diffusion models.** One stretching-rate threshold decides whether a
  phase-space diffusion model with an isotropic noise schedule has a reverse
  SDE, a well-posed likelihood objective, and an arrow of time.
- **Arrow of time.** Gaussian coarse-graining of a Hamiltonian ensemble gives a
  non-decreasing entropy for every initial state if and only if the resolution
  widens at least as fast as the flow stretches phase space (exact for linear
  flows; proven bounds and a conjecture for nonlinear ones).
- **Diósi–Penrose reduction.** Causal consistency of gravity-induced collapse
  and a mass scale that does not depend on the mass profile.
- **Carrier substrate.** A bandlimited-information framework for regular
  spacetime geometry and the quantum–classical boundary.

---

*Analysis and code are developed with the assistance of AI tools
(Google Gemini, OpenAI ChatGPT, Anthropic Claude); every stated result is
checked by the code in the corresponding repository.*
