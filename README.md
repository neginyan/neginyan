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
| *Beyond few harmonics: the lower side of the logarithmic law of the resolution gap for windows with a weak ripple* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23932698.svg)](https://doi.org/10.5281/zenodo.23932698) | [resolution-gap-weak-ripple](https://github.com/neginyan/resolution-gap-weak-ripple) | 20 |
| *Learned scores on the critically damped Langevin flow: a corrected sampler in 281 steps, and a metric-dependent fragility of the probability flow* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23899157.svg)](https://doi.org/10.5281/zenodo.23899157) | [cld-learned-score-samplers](https://github.com/neginyan/cld-learned-score-samplers) | 24 |
| *How fine can a hidden ripple be? A two-sided logarithmic law for the resolution gap of the arrow of time* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23746971.svg)](https://doi.org/10.5281/zenodo.23746971) | [resolution-gap-two-sided](https://github.com/neginyan/resolution-gap-two-sided) | 77 |
| *When the blur is slower than the flow: clipped and corrected samplers on the critically damped Langevin flow* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23689913.svg)](https://doi.org/10.5281/zenodo.23689913) | [cld-corrected-sampler](https://github.com/neginyan/cld-corrected-sampler) | 286 |
| *Is the resolution gap of the arrow of time uniform?* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23617343.svg)](https://doi.org/10.5281/zenodo.23617343) | [resolution-gap-log-law](https://github.com/neginyan/resolution-gap-log-law) | 65 + 12 |
| *Can a learned score see the margin of the arrow of time?* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23408213.svg)](https://doi.org/10.5281/zenodo.23408213) | [learned-score-arrow-of-time](https://github.com/neginyan/learned-score-arrow-of-time) | 68 |
| *The resolution gap in many degrees of freedom* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23371932.svg)](https://doi.org/10.5281/zenodo.23371932) | [resolution-gap-many-dof](https://github.com/neginyan/resolution-gap-many-dof) | 543 |
| *A resolution gap for the coarse-grained arrow of time in nonlinear Hamiltonian flows* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23320603.svg)](https://doi.org/10.5281/zenodo.23320603) | [resolution-gap-arrow-of-time](https://github.com/neginyan/resolution-gap-arrow-of-time) | 336 |
| *A stretching-rate threshold for phase-space diffusion models with isotropic marginal noise schedules* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23181225.svg)](https://doi.org/10.5281/zenodo.23181225) | [phase-space-diffusion-threshold](https://github.com/neginyan/phase-space-diffusion-threshold) | 113 |
| *Sharp criterion for the coarse-grained arrow of time in Hamiltonian dynamics* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23258135.svg)](https://doi.org/10.5281/zenodo.23258135) | [coarse-grained-arrow-of-time](https://github.com/neginyan/coarse-grained-arrow-of-time) | 33 |
| *Causal consistency of Diósi–Penrose reduction and a profile-independent mass scale M_P/√2* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23064513.svg)](https://doi.org/10.5281/zenodo.23064513) | [causal-consistency-dp-reduction](https://github.com/neginyan/causal-consistency-dp-reduction) | 55 |
| *The spacetime carrier substrate: bandlimited information, regular geometry, and a gravitational Heisenberg cut* | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22962656.svg)](https://doi.org/10.5281/zenodo.22962656) | [spacetime-carrier-substrate](https://github.com/neginyan/spacetime-carrier-substrate) | 177 |

#### Try it in your browser

Seven short notebooks reproduce a central result each in a few minutes on a CPU (Google Colab, no installation):

- **A corrected sampler in 281 steps.** One stored score network, one Brownian path: the Heun-type corrected sampler lands on the target at 281 steps, while Euler–Maruyama spreads every mode even at the same cost; and the handful of tail trajectories that break the probability-flow ODE, re-run with the learned and the exact score.
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neginyan/cld-learned-score-samplers/blob/main/demo/cld_learned_score_demo.ipynb)
- **How fine can a hidden ripple be?** The proved band for the resolution gap closes towards 1 from both sides as the blur shrinks, with the certified cells and the computed strips and combs inside it; a comb is a strip seen through a lens 256 times sharper.
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neginyan/resolution-gap-two-sided/blob/main/demo/hidden_ripple_demo.ipynb)
- **One line fixes the sampler.** The critically damped Langevin flow with an isotropic noise schedule: below the threshold the clipped sampler pulls every mode towards its centre, as the theory predicts, while the corrected sampler, one line different, lands on the target.
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neginyan/cld-corrected-sampler/blob/main/demo/cld_corrected_sampler_demo.ipynb)
- **How small can the gap get?** Ripple states recomputed down to σ = 10⁻⁹⁶ with an independent evaluator: their smallest gap shrinks like 1/√ln(1/σ), and stays above the proved lower bounds.
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neginyan/resolution-gap-log-law/blob/main/demo/resolution_gap_log_law.ipynb)
- **The arrow of time through a blurry lens.** Pendulums on their unstable top: with the blur fixed the coarse-grained entropy falls; blurring slightly slower than the stretching rate is still enough, because a finite resolution leaves a margin.
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neginyan/resolution-gap-arrow-of-time/blob/main/demo/arrow_of_time_demo.ipynb)
- **Sampling below the threshold.** A phase-space diffusion model sampled with the exact score: below the threshold the clipped reverse SDE shrinks every mode, the corrected sampler does not.
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neginyan/phase-space-diffusion-threshold/blob/main/demo/sampler_below_threshold.ipynb)
- **Many degrees of freedom, checked blind.** A search over all Gaussian states of two coupled pendulums, from random starts, lands on the matrix formula; widening along a momentum costs nothing; the sealed predictions are downloaded, hash-checked and recomputed.
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neginyan/resolution-gap-many-dof/blob/main/demo/resolution_gap_many_dof.ipynb)

#### In one line each

- **Beyond few harmonics.** The lower side of the log law extends to
  periodic windows with any number of harmonics whose ripple is weak or poor
  in low-frequency energy, for every state whose focus spans at least about
  0.7 ripple periods and for 10⁻⁴¹⁷ ≲ σ ≤ 10⁻²⁴ (computer-assisted proof,
  with an explicit bound on floating-point rounding in every cell); one of
  our own conjectures is refuted, and what remains open is listed from the
  nearest to the farthest.
- **Learned scores on the CLD flow.** With a learned score, a Heun-type
  corrected sampler is accurate in 281 steps in every metric tested; the
  learned probability-flow ODE breaks far more often when the metric lies
  above the threshold (10 of 12 networks against 3 of 16); thirteen of
  nineteen pre-registered predictions failed, and all are reported
  (numerical).
- **Two-sided log law.** On periodic windows (from strips to combs) the
  smallest resolution gap times √ln(1/σ) lies between 1 − 1.7 lnln/ln and
  1 + 6.0 lnln/ln for 10⁻¹⁰⁰⁰⁰⁰ ≤ σ ≤ 10⁻²⁴ (computer-assisted proof, under
  explicit assumptions); as σ → 0 it ends between 1 − ε̄ and 1 on every class
  whose remainder is bounded by ε̄, and tends to 1 along an explicit comb
  (proved); for general states one inequality remains conjectured.
- **CLD samplers.** On the critically damped Langevin flow with an isotropic
  noise schedule, the clipped reverse SDE is biased below the threshold and a
  corrected sampler, one line different, is exact (proved); the damage is
  mapped by exact error equations: a few per cent in typical settings, above
  10 % only when the final blur is comparable to the data scale or the mass is
  far from its default (numerical).
- **Log law.** The resolution gap is not uniform: ripple states shrink it to
  zero as σ → 0 (numerical), but only like 1/√ln(1/σ), and it cannot shrink
  faster (proved under one ratio condition, and without it for product states
  and for states without deep valleys; conjectured for all states).
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
