# FDS Final Project 2025 — X-ray Prohibited Item Classification

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/<USERNAME>/<REPO_NAME>/blob/main/<NOTEBOOK_PATH>.ipynb
)

Repository for the final project of the course *Fundamentals of Data Science*  
Master’s Degree in Data Science, Sapienza University of Rome.

## Project Overview

This project addresses a binary classification problem based on X-ray scanner imagery.  
The goal is to design and evaluate deep learning models capable of predicting whether an image contains prohibited items (label = 1) or is safe (label = 0).

## Dataset

The dataset is derived from the publicly available PIDray benchmark:

- Original repository: https://github.com/lutao2021/PIDray/tree/main  
- Due to storage constraints, the dataset is not included in this repository.  
  A shared Google Drive folder is available here:  
  https://drive.google.com/drive/folders/1zvMIc1bqteRN9Z36hHYpoTGoZArsh4mE

Only a subset of the original data is used:
- 6,000 SAFE images  
- 4,000 PROHIBITED images  

This split is intentionally slightly imbalanced to better reflect real-world distributions.

## Literature Reference

Zhang, L. et al. (2022).  
*PIDray: A Large-scale X-ray Benchmark for Real-World Prohibited Item Detection.*

## Methodology

The project methodology includes:
- Subset extraction and preprocessing  
- Train/validation splitting  
- Deep learning pipelines using convolutional neural networks (CNN)  
- Evaluation metrics: accuracy, precision, recall, F1-score, confusion matrix  
- Optional interpretability through Grad-CAM

Further implementation details will be added during project development.

## Results

To be added.

## Authors

- Francesco L.  
- Francesca D.  
- Emidio V.

## Requirements

See the `requirements.txt` file for Python dependencies.

## How to Run

Instructions will be added once the training pipeline is finalized.
