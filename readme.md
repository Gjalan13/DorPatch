# DorPatch Adversarial Patch Research Notebook

## Overview
This project notebook demonstrates the setup, execution, modification, and experimentation of the **DorPatch adversarial patch attack framework** using Python, PyTorch, and Google Colab.

The notebook focuses on:
- Setting up the DorPatch repository in Google Colab
- Downloading and preparing the ImageNet dataset
- Loading pretrained ImageNet models
- Running adversarial patch attacks
- Performing hyperparameter tuning experiments
- Visualizing attack results
- Extending DorPatch using a custom **DCT-based optimization approach**

---

## Features

### Environment Setup
- Mounts Google Drive in Google Colab
- Installs required dependencies
- Downloads DorPatch source files directly from GitHub
- Configures pretrained model directories

### Dataset Preparation
- Uses the ImageNet dataset from Kaggle
- Automatically prepares validation directories
- Creates symbolic links required by DorPatch
- Modifies dataset loading utilities for compatibility

### Model Support
- Uses pretrained ImageNet models
- Supports ResNet-based architectures
- Verifies CUDA/GPU availability for acceleration

### Adversarial Patch Experiments
- Executes DorPatch attacks using configurable parameters
- Supports density and structured sparsity tuning
- Measures:
  - Attack Success Rate
  - Runtime
  - Hyperparameter performance

### Visualization
- Displays random ImageNet samples
- Generates graphs and bar charts for experiment comparison
- Uses Matplotlib for visualization

### Novel Extension: DCT Optimization
This notebook introduces a custom extension using:
- Discrete Cosine Transform (DCT)
- Frequency-domain optimization
- Monkey-patching of the original DorPatch attack module

The DCT-based implementation explores alternative optimization strategies for generating adversarial patches.

---

## Technologies Used

- Python
- PyTorch
- torchvision
- NumPy
- Matplotlib
- Pillow
- SciPy
- Google Colab
- Kaggle API

---

## Project Structure

```text
DorPatch.ipynb
│
├── Environment Setup
├── Dependency Installation
├── DorPatch Repository Download
├── Dataset Preparation
├── Utility File Modifications
├── Hyperparameter Tuning
├── Result Visualization
├── DCT Optimization Module
└── Final Attack Execution
