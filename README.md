# Phase Transitions and Critical Phenomena: Interactive Lecture Notes

Interactive web companion to the graduate course on phase transitions and critical phenomena in the Department of Physics, Gyeongsang National University, following Nigel Goldenfeld's *Lectures on Phase Transitions and the Renormalization Group* (Addison-Wesley, 1992). The pages were created by Claude Opus 5.5 (Anthropic) based on Sang Hoon Lee's lecture notes. Each chapter is a single, self-contained HTML page that pairs the lecture notes with simulations and plots computed live in the browser.

## Chapters

Live pages (GitHub Pages). Start from the [course home page](https://lshlj82.github.io/phase-transition-and-critical-phenomena-GNU/).

| Chapter | Demo page | Source |
|---|---|---|
| 1. Introduction | [Open demo](https://lshlj82.github.io/phase-transition-and-critical-phenomena-GNU/ch01-introduction.html) | [`ch01-introduction.html`](ch01-introduction.html) |
| 2. How phase transitions occur in principle, Part 1 (§2.1–2.8) | [Open demo](https://lshlj82.github.io/phase-transition-and-critical-phenomena-GNU/ch02a-phase-transitions-in-principle.html) | [`ch02a-phase-transitions-in-principle.html`](ch02a-phase-transitions-in-principle.html) |
| 2. How phase transitions occur in principle, Part 2 (§2.8–2.14) | [Open demo](https://lshlj82.github.io/phase-transition-and-critical-phenomena-GNU/ch02b-symmetry-breaking-and-lattice-gases.html) | [`ch02b-symmetry-breaking-and-lattice-gases.html`](ch02b-symmetry-breaking-and-lattice-gases.html) |
| 3. How phase transitions occur in practice (§3.1–3.7 + appendix) | [Open demo](https://lshlj82.github.io/phase-transition-and-critical-phenomena-GNU/ch03-phase-transitions-in-practice.html) | [`ch03-phase-transitions-in-practice.html`](ch03-phase-transitions-in-practice.html) |
| 4. Critical phenomena in fluids (§4.1–4.5) | [Open demo](https://lshlj82.github.io/phase-transition-and-critical-phenomena-GNU/ch04-critical-phenomena-in-fluids.html) | [`ch04-critical-phenomena-in-fluids.html`](ch04-critical-phenomena-in-fluids.html) |
| 5. Landau theory, Part 1 (§5.1–5.3) | [Open demo](https://lshlj82.github.io/phase-transition-and-critical-phenomena-GNU/ch05a-landau-theory.html) | [`ch05a-landau-theory.html`](ch05a-landau-theory.html) |
| 5. Landau theory, Part 2 (§5.4–5.7) | [Open demo](https://lshlj82.github.io/phase-transition-and-critical-phenomena-GNU/ch05b-coarse-graining-and-correlations.html) | [`ch05b-coarse-graining-and-correlations.html`](ch05b-coarse-graining-and-correlations.html) |

The demo links assume the site is published with GitHub Pages; replace `lshlj82` and `phase-transition-and-critical-phenomena-GNU` throughout this file with your GitHub user name and repository name.

## Chapter 1: what's inside

The page follows the four sections of the notes and adds an interactive demo wherever a figure or equation invites one.

**1.1 Scaling and dimensional analysis**
- *Water waves.* The full dispersion relation $c^2 = (g\lambda/2\pi)\tanh(2\pi h/\lambda)$ against the shallow-water ($c=\sqrt{gh}$) and deep-water limits, plus a plot showing that every wavelength falls on the single scaling function $f(h/\lambda)$ from $c = (gh)^{1/2} f(h/\lambda)$. A toggle switches to the alternative convention $\tilde f(x) \sim x^{1/2}$.

**1.2 Power laws in statistical physics**
- *Coexistence-curve explorer.* How the exponent $\beta$ shapes the liquid–gas dome, and log–log slopes for SF₆ ($\beta = 0.327$), DyAlO₃ ($\beta = 0.311$), mean field ($\beta = 1/2$), and the 2D Ising model ($\beta = 1/8$).
- *2D Ising model.* Metropolis simulation with temperature and field controls, a live magnetization trace, and a one-click measurement of $\langle|m|\rangle(T)$ compared with Onsager's exact solution and mean-field theory.
- *Superfluid λ-transition.* A small power law $C \propto |t|^{-\alpha}$ versus a logarithm, showing why $\alpha = -0.013$ is so hard to distinguish from $\alpha = 0$ and why the heat capacity has a finite cusp.
- *Self-avoiding walks.* Pivot-algorithm sampling on the square and simple cubic lattices; fit $R \propto N^{\nu}$ yourself and compare with $\nu = 3/4$ (2D) and $\nu \approx 0.588$ (3D).
- *Dynamic critical phenomena.* The weak divergence of the shear viscosity, $\eta_s \propto t^{-0.03}$.

**1.3 Some important questions**
- *The thermodynamic limit.* Exact partition-function sums for the Curie–Weiss model with $N = 4$ to $4096$ spins: every finite-$N$ curve is smooth, and the kink in the order parameter and the jump in the heat capacity appear only as $N \to \infty$ (Question 0).
- A table of measured versus mean-field exponents (Question 2) and the three ingredients of a universality class (Question 3).

**1.4 Historical development**
- *Widom scaling collapse.* Adjust $\beta$ and $\delta$ until isotherms of a magnetic equation of state collapse onto $H = M^{\delta}\Phi(t/M^{1/\beta})$, with a numerical collapse score.
- A timeline from van der Waals (1873) to Wilson's renormalization group and the 1982 Nobel Prize, and a look at RG ideas beyond equilibrium.

A live 2D Ising lattice at the critical temperature runs in the page header. It evolves slowly on purpose so it does not distract from reading.

## Chapter 2, Part 1: what's inside

Part 1 covers §2.1–2.8: what a phase transition is, why it needs the thermodynamic limit, and how to decide whether one exists.

**2.1–2.2 Statistical mechanics and the thermodynamic limit**
- *Bulk and surface free energy.* Exact transfer-matrix results for open and periodic Ising chains: the open chain approaches $f_b$ as $1/N$ because of its two ends, the periodic ring exponentially fast. Readouts give $f_b$ and $f_s$.
- *Power-law interactions.* The bulk energy $E_b(R)$ for $U \propto r^{-\sigma}$ in $d$ dimensions, with presets for Coulomb/gravity, dipolar, and van der Waals forces, showing that the limit exists only for $\sigma > d$.

**2.3 Phase boundaries and phase transitions**
- *Crossing the phase diagram.* A mean-field magnet's $(T, H)$ phase diagram with a movable path: a jump in $m = -\partial f/\partial H$ below $T_c$ (first order), a diverging susceptibility at $T_c$ (continuous), and no singularity above $T_c$.
- *Correlation length vs system size.* How close to $T_c$ a sample of size $L$ can get before finite-size effects set in, from a 1 cm crystal ($|t| \sim 10^{-11}$) to a simulation box.

**2.5–2.6 The Ising model and its analytic properties**
- *Exact enumeration.* All $2^{16}$ states of a 4 × 4 periodic lattice summed exactly: $f$, $S$, $C_H$, and $M(H)$, with a live checklist confirming $f<0$, $S\ge0$, $C_H\ge0$, $\chi_T\ge0$, and $f(H)=f(-H)$. Every curve is smooth, because the system is finite.
- *Convexity.* The free energy of a mean-field magnet in the thermodynamic limit with a draggable chord; below $T_c$ the cusp at $H=0$ is the slope discontinuity that convexity allows.

**2.7 Symmetry properties**
- *Sublattice symmetry and frustration.* Ferromagnet vs antiferromagnet on square and triangular 4 × 4 lattices: identical free energies on the bipartite square lattice, different ones on the triangular lattice, where the frustrated antiferromagnet keeps a residual entropy.

**2.8 Existence of phase transitions**
- *Level crossing.* The lowest energy in each magnetization sector vs $H$, and the exact $M(H)$ of 16 spins sharpening into a step as $T \to 0$, with no thermodynamic limit needed.
- *Domain walls in one dimension.* $\Delta F = 2J - k_BT\ln N$ for a single wall, next to a slow heat-bath simulation of a 400-spin ring whose measured wall density is compared with the exact result.

The page header shows the space-time history of a 1D Ising chain, again deliberately slow.

## Chapter 2, Part 2: what's inside

Part 2 covers the rest of §2.8 through §2.14: why order survives in two dimensions, how a symmetric Hamiltonian ends up in an asymmetric state, why the system then cannot leave it, and why a fluid is a magnet in disguise.

**2.8 The Peierls argument**
- *Domain walls in two dimensions.* The wall free energy $\Delta F_n = [2J - k_BT\ln(z^*-1)]\,n$ at any temperature, and the resulting $T_c$ estimate against the exact value for the square, triangular, and honeycomb lattices. The coordination number that counts wall continuations is that of the dual lattice; with it, the estimate always falls below the exact $T_c$.

**2.9 Spontaneous symmetry breaking**
- *Two limits that do not commute.* Exact finite-$N$ Curie–Weiss results up to $N = 10^5$: every $M_N(H)$ passes through zero at $H = 0$, yet at any fixed small field $M_N \to M_s$ once $N \gtrsim k_BT/2HM_s$.
- *Sharp walls vs spread-out twists.* Why continuous symmetry needs $d > 2$: a twist spread over $w$ sites costs $\approx \pi^2J/2w$ per row, so system-spanning walls cost $L^{d-2}$ instead of $L^{d-1}$.

**2.10 Ergodicity breaking**
- *Reversal times.* Two-dimensional Ising models of side 4 to 16 run in parallel at $H=0$, $T<T_c$; the mean time between magnetization reversals grows exponentially with $L$ and is compared with the two-wall barrier $2\sigma L$ using Onsager's exact interfacial tension.
- *Spin-glass overlap distribution.* Exact $P(q)$ for a 16-spin Sherrington–Kirkpatrick model, single sample or averaged over 24, showing paramagnetic, ferromagnetic, and spin-glass shapes.
- *Quenched vs annealed, and the replica limit.* Free energies from the same samples, the exact annealed result, and $f_n = -k_BT\ln[Z^n]/nN$ as a smooth function of the replica number $n$.

**2.11–2.12 Fluids and lattice gases**
- *A lattice gas is an Ising magnet.* A grand-canonical simulation with live readouts of the mapping $J = -U_2/4$, $H = \mu/2 - zU_2/4$, plotted against the exact coexistence curve built from Onsager's spontaneous magnetization ($\beta = 1/8$).

**2.13–2.14** Exact vs approximate equivalence, a timeline of the thermodynamic limit (Kramers, the 1937 vote, Kramers–Wannier, Onsager), and whether quantum effects matter.

The page header shows a lattice gas at fixed density slowly condensing into liquid droplets.

## Chapter 3: what's inside

Chapter 3 puts the ideas of Chapter 2 to work: an exact solution of the one-dimensional Ising model by the transfer matrix, its correlations, the low-temperature expansion, and Weiss mean-field theory, with an appendix on the Ising model on networks.

**3.1–3.3 Exact solution in one dimension**
- *The transfer matrix, checked against brute force.* The matrix, its eigenvalues, the correlation length, and $\lambda_1^N + \lambda_2^N$ compared with a direct sum over all $2^N$ states of a ring (agreement to about $10^{-16}$). Plots show that the eigenvalues become degenerate only as $T\to0$ at $h=0$, the condition for a transition.

**3.4 Thermodynamic properties**
- *The exactly solved chain.* Energy, the Schottky-like heat-capacity peak near $k_BT\approx0.83J$, the susceptibility crossing over from Curie's law to $e^{2J/k_BT}/k_BT$, and $M(H)$ sharpening toward the $T=0$ step.

**3.5 Spatial correlations**
- *Exponential decay, measured and exact.* Heat-bath Monte Carlo on a 10,000-spin ring with block-averaged error bars, against $G(j) = (\tanh K)^j$; the correlation length $\xi = 1/\log(\lambda_1/\lambda_2)$ in zero and small fields.

**3.6 Low-temperature expansion**
- *Testing the series.* The cluster expansion against Onsager's exact free energy (numerical integration) on the square lattice, and its failure in $d=1$. In $d=2$ only, three-spin clusters and $2\times2$ blocks break as many bonds as two separated flipped spins, which changes the coefficient of $(w^2)^4$ from $-5/2$ to $+9/2$; the demo shows the resulting gain in accuracy.

**3.7 Mean-field theory**
- *Solving the self-consistency equation.* The graphical construction beside the variational free energy, with stable, unstable, metastable, and degenerate solutions identified.
- *Reading off the exponents.* Numerical solutions give $\beta = 1/2$, $\gamma = \gamma' = 1$, $\delta = 3$, the amplitude ratio 2, and the heat-capacity jump $\tfrac32k_B$.
- *The susceptibility sum rule.* Partial sums of $G(j)$ for the chain converge to $k_BT\chi_T = e^{2K}$.
- A table of mean-field, experimental, and Ising exponents in $d = 2, 3$, and Flory's $\nu = 3/(2+d)$ for self-avoiding walks.

**Appendix: the Ising model on networks**
- *Heterogeneous mean-field theory on scale-free networks.* For $p(k)\propto k^{-\gamma}$ with a natural cutoff: $m(T)$, the local exponent $\beta_{\rm eff}(t)$ approaching $1/(\gamma-3)$ for $3<\gamma<5$, and $T_c = J\langle k^2\rangle/\langle k\rangle$ against network size, diverging for $\gamma<3$.

The page header runs heat-bath dynamics on a 300-node Barabási–Albert network. Its temperature is scaled by the mean-field prediction; on this small sparse graph order actually sets in near 0.4–0.5 of that value, which the caption notes.

## Chapter 4: what's inside

Chapter 4 treats the liquid–gas critical point in the language of the earlier chapters.

**4.1 Thermodynamics and phase diagrams:** thermodynamic potentials and the thermodynamic square, the Clausius–Clapeyron relation, Landau's symmetry principle, two-phase coexistence, and Maxwell's equal-area construction.

**4.2 The van der Waals equation**
- *Critical constants from $a$ and $b$.* A calculator for $T_c$, $p_c$, $v_c$, preloaded with the book's argon fit and compared with experiment, with the universal ratio $p_cv_c/k_BT_c = 3/8$.
- *Isotherms and Maxwell's construction.* Reduced isotherms with the equal areas shaded and located numerically, the coexistence (binodal) and spinodal curves, and the vapor-pressure curve, with a live check that its slope equals $\Delta s/\Delta v$ (Clausius–Clapeyron).
- *The exponents, read off numerically.* From the full equation of state with numerical Maxwell construction: $\beta = 1/2$, $\gamma = \gamma' = 1$ with amplitude ratio 2, $\delta = 3$, and $C_p - C_V \propto (T-T_c)^{-1}$, matching mean-field theory for magnets.

**4.3–4.4 The critical point and density correlations:** exponent definitions for fluids, number fluctuations $\langle N^2\rangle - \langle N\rangle^2 = k_BT\rho^2V\kappa_T$ via Jacobians, the compressibility sum rule, and critical opalescence.
- *Measuring the structure factor.* A 128 × 128 lattice gas at its critical density (Wolff cluster updates), with $S(k)$ from a 2D FFT, an Ornstein–Zernike fit for $\xi$, and the $k^{-7/4}$ law expected at $T_c$ in two dimensions.

**4.5 Measuring critical exponents**
- *Try to measure α.* Synthetic heat-capacity "data" with a true $\alpha = 0.11$, a correction to scaling, a smooth background, instrumental rounding, and an adjustable error in $T_c$. Students choose a fit window and compare the naive slope with the local exponent.

The page header is a slowed-down molecular-dynamics simulation of 256 Lennard-Jones particles in two dimensions, with liquid droplets coexisting with vapor below $k_BT_c \approx 0.46\epsilon$.

## Chapter 5, Part 1: what's inside

Part 1 covers order parameters, the common structure of mean-field theories, and phenomenological Landau theory.

- *Two theories, one Landau function (§5.2).* The exact Weiss and van der Waals equations of state, each rescaled so that its leading terms read $y = tx + x^3$, collapse onto the Landau form near the critical point; a second panel shows the higher-order terms that distinguish them.
- *The Landau free energy explorer (§5.3).* An interactive version of the book's Figure 5.1: $\mathcal L = at\eta^2 + \tfrac12b\eta^4 + C\eta^3 - H\eta$ with its global and metastable minima, the equilibrium $\eta(t)$, and $\mathcal L_{\min}(t)$ with its second derivative. The continuous transition shows the heat-capacity jump; a cubic term gives a first-order jump at $t_1 = C^2/2ab$ with $\eta(t_1) = -C/b$.
- *A non-analytic Landau term from network heterogeneity (§5.3 aside).* Adding $C|\eta|^{\lambda-1}$ for degree exponent $\lambda$: no transition for $2<\lambda<3$, $\beta = 1/(\lambda-3)$ for $3<\lambda<5$, and $\beta = 1/2$ for $\lambda>5$, with a numerical fit of $\beta$.

The page header shows a ball relaxing in the Landau potential as the temperature slowly cycles through $T_c$, falling into one of the two wells at random each time.

## Chapter 5, Part 2: what's inside

Part 2 covers coarse graining, the meaning of the Landau free energy, and the correlation functions of Landau theory, and closes with a review of the semester.

- *A non-convex Landau function and a convex Gibbs function (§5.5).* For the Curie–Weiss magnet both are exact: the constrained free energy $\mathcal L(m)$ from the partial trace is a double well below $T_c$, while the Gibbs function $\Gamma_N(m)$ from the full trace is convex for every $N$ and converges to the convex hull of $\mathcal L$, flat between $\pm m_s$.
- *Solving the Landau equation (§5.7).* Gradient-descent relaxation of the one-dimensional Landau functional: a domain wall converging to $\eta_s\tanh(x/2\xi_<)$, and the response to a point field decaying as $e^{-|x|/\xi}$, with fitted decay lengths matching $\xi_> = (\gamma/2at)^{1/2}$ and $\xi_< = (-\gamma/4at)^{1/2}$.
- *The Ornstein–Zernike correlation function in $d$ dimensions (§5.7).* $G(r)$ from the modified Bessel function $K_{(d-2)/2}$, evaluated numerically for any real $d$, with its critical and long-distance limits, and the Lorentzian $\hat G(k)$.

The page header shows an Ising model near $T_c$ beside its coarse-grained magnetization field, with a selectable block size $\Lambda^{-1}$. A closing section reviews the semester and points ahead to the renormalization group.

## Running locally

No build step and no dependencies to install. Clone the repository and open the HTML file in any modern browser:

```bash
git clone https://github.com/lshlj82/phase-transition-and-critical-phenomena-GNU.git
cd phase-transition-and-critical-phenomena-GNU
open ch01-introduction.html        # macOS
xdg-open ch01-introduction.html    # Linux
start ch01-introduction.html       # Windows
```

An internet connection is needed the first time for the web fonts and for [KaTeX](https://katex.org/) (loaded from jsDelivr), which typesets the equations. Everything else, including all simulations, runs offline in plain JavaScript.

## Publishing with GitHub Pages

1. Push the repository to GitHub.
2. Go to **Settings → Pages**, choose **Deploy from a branch**, and select `main` with the `/ (root)` folder.
3. Each chapter will be served at a URL such as `https://lshlj82.github.io/phase-transition-and-critical-phenomena-GNU/ch01-introduction.html`.

The landing page `index.html` is served at `https://lshlj82.github.io/phase-transition-and-critical-phenomena-GNU/` and links to every chapter.

## Repository layout

```
.
├── README.md
├── index.html                                     # Landing page linking every chapter
├── ch01-introduction.html                         # Chapter 1
├── ch02a-phase-transitions-in-principle.html     # Chapter 2, Part 1 (§2.1–2.8)
├── ch02b-symmetry-breaking-and-lattice-gases.html # Chapter 2, Part 2 (§2.8–2.14)
├── ch03-phase-transitions-in-practice.html        # Chapter 3 (§3.1–3.7 + appendix)
├── ch04-critical-phenomena-in-fluids.html         # Chapter 4 (§4.1–4.5)
├── ch05a-landau-theory.html                       # Chapter 5, Part 1 (§5.1–5.3)
└── ch05b-coarse-graining-and-correlations.html    # Chapter 5, Part 2 (§5.4–5.7) and semester review
```

Each chapter page is intentionally self-contained (HTML, CSS, and JavaScript in one file) so it can be opened directly, emailed to students, or dropped into a course website without a build process.

## Technical notes

- **Rendering:** HTML5 canvas for all plots and lattices, using a small built-in plotting helper (linear and logarithmic axes, legends, reference lines). No charting library.
- **Ising model:** single-spin Metropolis updates at a user-adjustable rate (sweeps per second) for the interactive demo, so critical slowing down is visible. The header lattice is prepared at $T_c$ with Wolff cluster updates and then evolves gently at a fixed, slow rate (about six Metropolis sweeps per second).
- **Self-avoiding walks:** the pivot algorithm with the 8 (2D) or 48 (3D) lattice symmetries and hash-set self-intersection checks; separate Markov chains for each chain length.
- **Exact enumeration (Ch. 2):** all $2^{16}$ configurations of 4 × 4 periodic square and triangular lattices are enumerated once at page load into a table of (bond sum, magnetization, count), from which every thermodynamic quantity at any $T$ and $H$ follows exactly.
- **Transfer matrices (Ch. 2):** open-chain and periodic-ring partition functions of the 1D Ising model computed exactly with rescaled matrix products.
- **Spin-glass enumeration (Ch. 2, Part 2):** energies of all $2^{16}$ states of each Sherrington–Kirkpatrick sample are generated with a Gray-code walk (one spin flip per step), and the overlap distribution over all $2^{32}$ pairs of states is obtained exactly from the XOR autocorrelation of the Boltzmann weights via two Walsh–Hadamard transforms. Disorder samples use a seeded random-number generator, so they are reproducible.
- **Lattice-gas dynamics (Ch. 2, Part 2):** particle-conserving (Kawasaki) exchange moves for the fixed-density header, and grand-canonical Metropolis moves of the equivalent Ising model for the interactive demo.
- **Onsager free energy (Ch. 3):** the exact square-lattice free energy is evaluated by midpoint integration of $\tfrac12\iint\ln[\cosh^2 2K - \sinh 2K(\cos\theta_1+\cos\theta_2)]$ over $[0,\pi]^2$, accurate enough to resolve the $x^8$ term of the low-temperature series.
- **Mean-field solutions (Ch. 3):** the self-consistency equation is solved by geometric bisection rather than fixed-point iteration, which converges too slowly near $T_c$ to give correct exponents.
- **Networks (Ch. 3):** a seeded Barabási–Albert graph laid out once by a Fruchterman–Reingold force simulation; heterogeneous mean-field sums use exact degree sums up to $k = 3000$ and a log-spaced integral beyond, so cutoffs up to $N = 10^{18}$ are cheap.
- **Van der Waals (Ch. 4):** reduced units throughout; spinodals found by bisection of $4\tau\nu^3 = (3\nu-1)^2$ on either side of $\nu = 1$, and the coexistence pressure by bisection on the equal-area condition using the closed-form integral of $\pi(\nu)$. The critical isotherm uses the exact form $\pi - 1 = -3\phi^3/[(2+3\phi)(1+\phi)^2]$ to avoid floating-point cancellation.
- **Molecular dynamics (Ch. 4):** velocity-Verlet integration of a truncated Lennard-Jones fluid ($r_c = 2.5\sigma$) with a Berendsen thermostat.
- **Structure factor (Ch. 4):** radix-2 FFTs of the occupation numbers, radially binned and time-averaged.
- **Landau equation (Ch. 5, Part 2):** explicit gradient-descent relaxation of the one-dimensional Landau functional on a 401-point grid, with fixed bulk values at the ends for the domain wall and reflecting ends for the point field.
- **Bessel functions (Ch. 5, Part 2):** $K_\nu(x)$ from the integral representation $\int_0^\infty e^{-x\cosh u}\cosh\nu u\,du$ by the trapezoid rule, so non-integer dimensions work; Lanczos approximation for $\Gamma$.
- **Curie–Weiss model:** exact summation of $Z_N = \sum_k \binom{N}{k} e^{\beta J (2k-N)^2/2N}$ using log-factorials and log-sum-exp for numerical stability.
- **Accessibility and performance:** high-contrast palettes for light and dark color schemes (spins are drawn in deep navy and bright yellow so the two states differ strongly in lightness, not only hue); the scheme follows the operating-system setting; animation speeds are deliberately calm; simulations pause when scrolled out of view; the header animation starts paused when the user prefers reduced motion; layouts reflow down to phone widths.

## References

- N. Goldenfeld, *Lectures on Phase Transitions and the Renormalization Group* (Addison-Wesley, 1992).
- S. G. Brush, "History of the Lenz–Ising model," *Rev. Mod. Phys.* **39**, 883 (1967).
- R. Peierls, "On Ising's model of ferromagnetism," *Proc. Cambridge Philos. Soc.* **32**, 477 (1936).
- H. A. Kramers and G. H. Wannier, "Statistics of the two-dimensional ferromagnet," *Phys. Rev.* **60**, 252 and 263 (1941).
- T. D. Lee and C. N. Yang, "Statistical theory of equations of state and phase transitions. II. Lattice gas and Ising model," *Phys. Rev.* **87**, 410 (1952).
- D. Sherrington and S. Kirkpatrick, "Solvable model of a spin-glass," *Phys. Rev. Lett.* **35**, 1792 (1975).
- M. Mézard, G. Parisi, and M. A. Virasoro, *Spin Glass Theory and Beyond* (World Scientific, 1987).
- M. Dresden, "Kramers's contributions to statistical mechanics," *Physics Today* **41**(9), 26 (1988).
- C. Domb, "On the theory of cooperative phenomena in crystals," *Adv. Phys.* **9**, 149 (1960).
- J. C. Le Guillou and J. Zinn-Justin, "Critical exponents from field theory," *Phys. Rev. B* **21**, 3976 (1980).
- S. H. Lee, M. Ha, H. Jeong, J. D. Noh, and H. Park, "Critical behavior of the Ising model in annealed scale-free networks," *Phys. Rev. E* **80**, 051127 (2009).
- S. N. Dorogovtsev, A. V. Goltsev, and J. F. F. Mendes, "Critical phenomena in complex networks," *Rev. Mod. Phys.* **80**, 1275 (2008).
- E. A. Guggenheim, "The principle of corresponding states," *J. Chem. Phys.* **13**, 253 (1945).
- B. Smit and D. Frenkel, "Vapor–liquid equilibria of the two-dimensional Lennard-Jones fluid(s)," *J. Chem. Phys.* **94**, 5663 (1991).
- L. D. Landau and E. M. Lifshitz, *Statistical Physics, Part 1*, 3rd ed. (Pergamon, 1980).
- A. V. Goltsev, S. N. Dorogovtsev, and J. F. F. Mendes, "Critical phenomena in networks," *Phys. Rev. E* **67**, 026123 (2003).
- L. P. Gor'kov, "Microscopic derivation of the Ginzburg–Landau equations in the theory of superconductivity," *Sov. Phys. JETP* **9**, 1364 (1959).
- P. M. Chaikin and T. C. Lubensky, *Principles of Condensed Matter Physics* (Cambridge University Press, 1995).
- R. J. Baxter, *Exactly Solved Models in Statistical Mechanics* (Academic Press, 1982).
- G. H. Wannier, "Antiferromagnetism. The triangular Ising net," *Phys. Rev.* **79**, 357 (1950).
- J. Fröhlich and T. Spencer, "The phase transition in the one-dimensional Ising model with $1/r^2$ interaction energy," *Commun. Math. Phys.* **84**, 87 (1982).
- G. I. Barenblatt, *Scaling* (Cambridge University Press, 2003).
- D. V. Schroeder, *An Introduction to Thermal Physics* (Addison-Wesley, 2000).
- L. Onsager, "Crystal statistics. I. A two-dimensional model with an order-disorder transition," *Phys. Rev.* **65**, 117 (1944).
- U. Wolff, "Collective Monte Carlo updating for spin systems," *Phys. Rev. Lett.* **62**, 361 (1989).
- N. Madras and A. D. Sokal, "The pivot algorithm: a highly efficient Monte Carlo method for the self-avoiding walk," *J. Stat. Phys.* **50**, 109 (1988).

## Acknowledgments and disclaimer

These pages were created by Claude Opus 5.5 (Anthropic) based on Sang Hoon Lee's lecture notes on Goldenfeld's textbook, for the graduate course of the Department of Physics, Gyeongsang National University. The text is a paraphrase written for teaching; it does not reproduce the book, and this project is not affiliated with or endorsed by the author or publisher. Experimental exponent values are those quoted in the notes.

## License

Choose a license before publishing; for course material a common pairing is [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) for the text and [MIT](https://opensource.org/license/mit) for the code.
