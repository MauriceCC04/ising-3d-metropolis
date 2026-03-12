# 3D Ising Model — Metropolis Monte Carlo Simulation (Notebook)

This project simulates the **3D Ising model** using the **Metropolis Monte Carlo algorithm** and analyzes how **magnetization changes with temperature** under different settings (lattice size, coupling strength, external field).

The implementation and analysis are contained in a single Jupyter notebook.

## What this notebook does
- Defines the 3D Ising Hamiltonian:
  - coupling strength `J` (ferromagnetic / non-interacting / antiferromagnetic)
  - external field `h`
- Runs Metropolis sampling across multiple temperatures and lattice sizes
- Visualizes magnetization behavior and discusses phase-transition behavior

## Key observations (from the notebook)
- For **ferromagnetic coupling (J = 1, h = 0)**: behavior consistent with a second-order phase transition around **T ≈ 4.5**
- For **J = 0**: no cooperative behavior / no phase transition
- For **J = -1**: antiferromagnetic ordering tendencies
- For **h ≠ 0**: explicit symmetry breaking; magnetization biased by field direction

## Repo structure
- `ising-3d-metropolis.ipynb` *(rename from `Project.ipynb` recommended)* — full implementation + analysis
- `.gitignore`, `.gitattributes`

> Recommended: do **not** include course handouts/instructions PDFs in a public repo.

## How to run

### Option A — Run locally
1. Create an environment (recommended) and install dependencies:

```bash
pip install numpy matplotlib numba tqdm jupyter
````

2. Start Jupyter and open the notebook:

```bash
jupyter notebook
```