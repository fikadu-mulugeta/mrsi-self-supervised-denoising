# Self-Supervised Denoising of MRSI Data

This repository contains the implementation developed for my master's thesis on self-supervised denoising of Magnetic Resonance Spectroscopic Imaging (MRSI) data using deep learning techniques.

The project focuses on improving MRSI signal quality through a two-stage denoising pipeline involving:
- Spatial-domain denoising
- Spectral-domain denoising
- Reconstruction and evaluation of denoised spectra

The framework was developed using Python and PyTorch.

---

# Project Overview

Magnetic Resonance Spectroscopic Imaging (MRSI) often suffers from low signal-to-noise ratio (SNR), which negatively affects spectral quality and metabolite analysis.

This project investigates a self-supervised learning approach for denoising MRSI data without requiring fully clean target data.

The proposed pipeline includes:
1. Spatial denoising
2. Spectral denoising
3. Reconstruction of denoised outputs
4. Quantitative and qualitative evaluation

The workflow was evaluated using Leave-One-Out Cross-Validation (LOOCV).

---

# Repository Structure

```text
mrsi-self-supervised-denoising/
│
├── notebooks/
│   └── mrsi_self_supervised_denoising.ipynb
│
├── requirements.txt
├── LICENSE
└── README.md
```

---

# Methods

## 1. Spatial Denoising

A self-supervised spatial denoising model is trained to reduce noise while preserving spatial structure in MRSI data.

## 2. Spectral Denoising

A spectral-domain denoising model is applied to improve spectral fidelity and suppress residual noise.

## 3. Reconstruction

The denoised outputs are reconstructed and evaluated against reference spectra using quantitative and qualitative analysis.

---

# Technologies Used

- Python
- PyTorch
- NumPy
- SciPy
- Matplotlib
- Scikit-learn
- Scikit-image
- Jupyter Notebook

---

# Dataset and Output Availability

The MRSI dataset and generated outputs used in this project are not publicly distributed due to privacy and institutional data-sharing restrictions.

Data and selected outputs may be shared upon reasonable request and subject to approval and applicable data-sharing policies.

---

# Installation

## Clone the Repository

```bash
git clone https://github.com/fikadu-mulugeta/mrsi-self-supervised-denoising.git
cd mrsi-self-supervised-denoising
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebooks/mrsi_self_supervised_denoising.ipynb
```

---

# Results

The notebook includes:
- Spatial denoising examples
- Spectral denoising comparisons
- Reconstructed spectra visualizations
- Quantitative evaluation metrics
- Before/after comparisons

---

# Future Improvements

Planned future improvements include:
- modularization into reusable Python modules
- training script separation
- reusable data loaders
- model packaging and reproducibility improvements

---

# Notes

This repository is intended for research and educational purposes.

Some preprocessing and dataset-specific steps may require adaptation depending on the available MRSI dataset structure.

---

# Author

Fikadu Mulugeta Gassa

Master's Thesis Project

Università Politecnica delle Marche (UNIVPM), Ancona, Italy
Medical University of Vienna (MedUniWien), Vienna, Austria
