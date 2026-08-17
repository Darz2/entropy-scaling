# Entropy scaling

Molecular simulation and analysis code for **excess entropy** computed by integrating the radial distribution function, using the **Wang–Frenkel (WF) potential**.

This is the code behind the study of finite-size effects in excess entropy obtained from RDF integration. The WF parameters used here are α = 1 and λ = 0.5.

## Contents

- `MC/` — Monte Carlo simulation inputs and run scripts
- `WF/` — Wang–Frenkel potential definition and parameters
- `GRintegrate/` — excess entropy by direct integration of g(r)
- `GRintegrate-derivatives/` — derivative-based variant of the integration
- `GRanalytical/` — analytical reference expressions for g(r)
- `test/` — test cases

## Background

The excess entropy of a fluid can be obtained from the pair distribution function via the two-body term of the entropy expansion. Because g(r) is computed in a finite periodic box, the resulting excess entropy carries a system-size dependence. This repository contains the simulations and integration routines used to quantify and correct that dependence.

## Citation

> Raju, D.; et al. *Finite-size effects of the excess entropy computed from integrating the radial distribution function.* Molecular Physics (2025). https://doi.org/10.1080/00268976.2025.2456115

## License

MIT — see [LICENSE](LICENSE).
