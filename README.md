<div align="center">

# 🧩 Sudoku-Inspired CT Image Reconstruction

**A constraint-based approach to reconstructing missing CT image regions**

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Research-yellow)

</div>

---

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Methodology](#methodology)
- [Performance Evaluation](#performance-evaluation)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Future Improvements](#future-improvements)
- [License](#license)

---

## Project Overview

This project explores a **Sudoku-inspired approach** to CT (Computed Tomography) image reconstruction. The core idea is to reconstruct missing image regions by treating the image as a grid of patches and applying **constraint-based logic**, inspired by Sudoku-solving strategies, to determine the most suitable reconstruction for each patch.

The project investigates how logical constraints combined with patch similarity can preserve anatomical structures while minimizing reconstruction errors.

---

## Features

- Constraint-based CT image reconstruction
- Patch similarity matching for missing regions
- Bilateral filtering for artifact reduction
- Quantitative evaluation using PSNR, SSIM, and MSE
- Visual comparison with error analysis and heatmaps

---

## Methodology

The reconstruction pipeline consists of the following steps:

| Step | Description |
|:----:|-------------|
| 1 | Divide the CT image into small grid patches |
| 2 | Identify missing or corrupted image regions |
| 3 | Reconstruct missing patches using a Sudoku-inspired constraint strategy and patch similarity matching |
| 4 | Apply bilateral filtering to reduce block artifacts while preserving anatomical edges |
| 5 | Evaluate the reconstructed image using quantitative image quality metrics |

---

## Performance Evaluation

Reconstruction quality is assessed using three standard image quality metrics:

| Metric | Description |
|--------|-------------|
| **PSNR** (Peak Signal-to-Noise Ratio) | Measures reconstruction fidelity |
| **SSIM** (Structural Similarity Index) | Evaluates structural similarity between original and reconstructed images |
| **MSE** (Mean Squared Error) | Measures the average reconstruction error |

---

## Results

The figure below compares the original CT image with the reconstructed image, the absolute difference map, and the reconstruction error heatmap.

<p align="center">
  <img src="Figures/IMG_0370.png" width="850">
</p>

---

## Technologies Used

- Python
- NumPy
- OpenCV
- Matplotlib
- scikit-image

---

## Future Improvements

- [ ] Improve patch matching using feature-based similarity
- [ ] Reduce block artifacts with adaptive reconstruction strategies
- [ ] Compare the proposed approach with conventional image reconstruction techniques
- [ ] Investigate machine learning-based optimization for patch selection

---

## License

This project is released under the **MIT License**.
