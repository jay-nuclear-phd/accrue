# ACCRUE Figures Reproduction

This repository accompanies the paper:

**_Advancing Uncertainty Reduction in Nuclear Criticality Safety: Application of ACCRUE Relevance Index_**

It contains code and a single notebook to **reproduce the figures** used in the manuscript.

## Contents

- `reproducing_figures.ipynb` — the main, ordered notebook that generates the figures.  
- `requirements.txt` — pinned Python packages for a clean, reproducible environment.  
- `data/` — expected location for input data files used by the notebook (e.g.  
  `data/keff_data_summary.xlsx`, `data/benchmark_620.pkl`).

> If the data files are not part of the repo, place them under `data/` with the exact filenames/paths referenced in the notebook.

## Quick Start

### 1) Create an environment (optional but recommended)
```bash
# Python 3.10+ recommended
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS / Linux
source .venv/bin/activate
```

### 2) Install dependencies
```bash
pip install -r requirements.txt
```

### 3) Reproduce the figures
Open the notebook and **run all cells in order**:

```bash
# Option A: classic Jupyter
jupyter notebook reproducing_figures.ipynb

# Option B: JupyterLab
jupyter lab reproducing_figures.ipynb

# Option C: VS Code
# Open the repo folder in VS Code and run the notebook interactively
```

> The notebook is written to be executed **top-to-bottom**. If you change any parameters or file paths, re-run the earlier cells that define them.

## Notes

- The workflow uses Times New Roman and mathtext settings in Matplotlib so that figure typography matches the paper.  
- Random seeds are set where relevant to ensure reproducibility of stochastic examples.  
- Some figures expect data at fixed paths (e.g., `data/keff_data_summary.xlsx`, `data/benchmark_620.pkl`). Adjust paths in the notebook if your files live elsewhere.

## Citation

If you use this repository or reproduce the figures, please cite:

> _Advancing Uncertainty Reduction in Nuclear Criticality Safety: Application of ACCRUE Relevance Index_, 2025.  
> (Add full journal / DOI information will be added when available.)

## License

CC0 1.0 Universal
