# MHIST Research

This repository contains the workspace for MHIST image classification experiments.

## Project Structure

```text
MHIST-Research/
├── data/
│   ├── raw/
│   ├── processed/
│   └── metadata/
├── notebooks/
│   ├── 01_exploration.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_baseline.ipynb
│   ├── 04_lightweight_models.ipynb
│   ├── 05_robustness.ipynb
│   ├── 06_gradcam.ipynb
│   └── 07_agreement_analysis.ipynb
├── src/
│   ├── dataset.py
│   ├── preprocessing.py
│   ├── train.py
│   ├── evaluate.py
│   ├── robustness.py
│   ├── gradcam.py
│   └── metrics.py
├── models/
│   ├── checkpoints/
│   └── configs/
├── results/
│   ├── figures/
│   ├── tables/
│   └── predictions/
└── requirements.txt
```

Install the initial dependencies with:

```bash
pip install -r requirements.txt
```