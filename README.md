# DATA1030 — Final project repository

This repository contains course materials and a capstone-style analysis for the DATA1030 (Fall 2025) project: exploratory analysis, preprocessing, models, figures, and a short report describing the results.

- Course / Canvas: https://canvas.brown.edu/courses/1099954

This README explains how the project is organized and how to reproduce the environment used to develop the notebooks.

**Repository layout**

```
.
├── data/         # raw and preprocessed datasets (if small enough for GitHub)
├── figures/      # generated figures, plots, and visual assets
├── results/      # saved models, predictions, and evaluation output
├── report/       # final report (PDF) and supplementary documents
├── src/          # source code and notebooks (analysis & experiments)
├── .gitignore
├── LICENSE
└── README.md
```

Notes:
- If your raw dataset is too large to store on GitHub, keep a small sample in `data/` and add a download link (or scripts) to reproduce the full dataset locally.

**Quick start (reproducible environment)**

1. Install conda/miniconda and create the environment from `environment.yml`:

```bash
conda env create -f environment.yml
conda activate data1030
```

2. Start JupyterLab (or Jupyter Notebook) to run the notebooks in `src/`:

```bash
jupyter lab
```

3. Reproduce figures and results by opening the relevant notebook(s) in `src/`.

**Python & major package versions (used while developing)**
- Python 3.10
- numpy >= 1.26
- pandas >= 2.2
- scikit-learn >= 1.3
- matplotlib >= 3.7
- seaborn >= 0.12
- shap (via pip)

Exact versions are provided in `environment.yml` for reproducibility.

**Where to find things**
- Data: `data/`
- Figures: `figures/`
- Results (predictions, saved model weights): `results/`
- Final report PDF (and supplementary files): `report/`
- All code, experiments and notebooks: `src/` (some legacy notebooks may still be in the repo root or `1030HW/` — consider moving them into `src/` for a clean structure)

**License**
This project is licensed under the MIT License — see `LICENSE` for details.

If you want me to move the notebooks into `src/` and reorganize files now, tell me and I will perform the moves for you.

---
If anything here should follow a different convention or you'd like a different license, tell me which and I'll update the repo accordingly.
