# Statistical-modeling
Coursework from the university module Statistical Modeling — a single in-depth Jupyter notebook building pseudo-random generation, randomness testing, random-variable simulation, Monte Carlo integration, and Markov chains from first principles in Python.

#Overview

This notebook works through the full stochastic-simulation pipeline, deriving each method from its theory before implementing it. The emphasis is on understanding why each technique works, not just calling a library function — most generators and tests are built from scratch with NumPy and math.

# Topics covered
 
1. **Pseudo-random number generation** — the Linear Congruential Method with maximal period. Parameters are chosen rigorously: the increment `c` via the serial-correlation criterion, the multiplier `a` via the maximal-period theorems and "potency" analysis.
2. **Randomness testing** — generated sequences are validated with the *maximum test* and a *permutation (runs) test*, evaluated against the chi-square distribution.
3. **Random-variable simulation** — generating variates from target distributions: the F-distribution (built up from chi-square, which is in turn built from exponential variates), and the exponential distribution via the inverse-transform method. Results are compared against theoretical density curves.
4. **Monte Carlo integration** — estimating definite integrals by sampling, including the use of different sampling densities (importance sampling) to reduce error.
5. **Markov chains** — simulating a chain from a chosen transition matrix and initial distribution, driven by the custom-built random sequence.

# Note
 
Academic coursework, shared as part of my data-analysis portfolio.
