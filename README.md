# FDS Final Project 2025 — Optimization Process for Airport Security

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WQ8QMyDFFhGe1We4INtXWm7yOYNEMt0S?usp=sharing)


Repository for the final project of the course *Fundamentals of Data Science*  
Master’s Degree in Data Science, Sapienza University of Rome.

## Project Overview

This project addresses a classification problem based on X-ray scanner imagery.  
The goal is to design and evaluate deep learning models capable of predicting whether an image contains prohibited items and where is located that item.

## Dataset

The dataset is derived from the publicly available PIDray benchmark:

- Original repository: https://github.com/lutao2021/PIDray/tree/main  
- Due to storage constraints, the dataset is not included in this repository.  
  A shared Google Drive folder is available here:  
  https://drive.google.com/drive/folders/1zvMIc1bqteRN9Z36hHYpoTGoZArsh4mE

Only a subset of the original data is used, ~10000 images.


## Literature Reference

Zhang, L. et al. (2022).  
*PIDray: A Large-scale X-ray Benchmark for Real-World Prohibited Item Detection.*

## Methodology

The project methodology includes:
- Subset extraction and preprocessing  
- Train/validation splitting  
- Deep learning pipelines using convolutional neural networks (CNN with RESNET)
- YOLOv8 Model application, with Hyperparameter Research
- Evaluation metrics: accuracy, precision, recall, F1-score, confusion matrix  
- Optional interpretability through Grad-CAM [not completed]

Further implementation details will be added during project development.

## Results

The high quality of the dataset, highlighted during the exploratory analysis, motivated us to move toward an object detection approach. The multilabel classification results obtained with ResNet showed very strong performance, indicating that the data contained rich and informative visual patterns. For this reason, we adopted YOLO for object detection.
While the overall results were good, the model struggled with rare classes such as guns and scissors, due to severe class imbalance. To address this issue, we performed hyperparameter research suited to our dataset, which allowed us to improve the detection performance and obtain better final results.


## Authors

- Francesco La Piana
- Francesca Di Cricio
- Emidio Veccia

## Requirements

See the `requirements.txt` file for Python dependencies.

<img width="482" height="703" alt="image" src="https://github.com/user-attachments/assets/ec463c70-9d86-4c52-8733-f99ee0d56cf6" />
