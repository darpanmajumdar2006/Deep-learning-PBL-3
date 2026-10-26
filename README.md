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

## Results

Generated tables are stored in `MHIST-Research/results/tables/`, and plots are stored in `MHIST-Research/results/figures/`.
Per-image test predictions for all four models are saved in [`test_set_predictions.csv`](MHIST-Research/results/predictions/test_set_predictions.csv).

The Grad-CAM notebook includes one test image from each true class and visualizes each of the four trained models. The resulting overlays are saved here:

| Model | HP sample | SSA sample |
|---|---|---|
| ResNet18 | [Grad-CAM](MHIST-Research/results/figures/gradcam_resnet18_hp.png) | [Grad-CAM](MHIST-Research/results/figures/gradcam_resnet18_ssa.png) |
| EfficientNet-B0 | [Grad-CAM](MHIST-Research/results/figures/gradcam_efficientnet_b0_hp.png) | [Grad-CAM](MHIST-Research/results/figures/gradcam_efficientnet_b0_ssa.png) |
| MobileNetV3-Small | [Grad-CAM](MHIST-Research/results/figures/gradcam_mobilenetv3_small_hp.png) | [Grad-CAM](MHIST-Research/results/figures/gradcam_mobilenetv3_small_ssa.png) |
| ShuffleNetV2-x0.5 | [Grad-CAM](MHIST-Research/results/figures/gradcam_shufflenetv2_x0_5_hp.png) | [Grad-CAM](MHIST-Research/results/figures/gradcam_shufflenetv2_x0_5_ssa.png) |
