# Fetal-Health-Classification-with-Python

## Abstract

This project aims to classify fetal health to prevent child and maternal mortality using features extracted from Cardiotocogram (CTG) exams. The primary challenge is dealing with dataset imbalance.

## About the Dataset

### Context

Reducing child mortality is crucial for human progress, and maternal mortality is also a significant concern. Cardiotocograms (CTGs) provide a cost-effective means to assess fetal health, enabling early intervention to prevent child and maternal mortality.

### Data

The dataset contains 2126 records of features extracted from CTG exams, classified into three categories:

1. Normal
2. Suspect
3. Pathological

## Results and Recommendations

Due to dataset imbalance, various models and sampling methods were employed to achieve the best results. Here are the findings:

### Sampling Methods

1.Random Sampling
2. OverSampling
3. UnderSampling

### Models

1. Random Forest
2. K-Nearest Neighbors (KNN)
3. Decision Tree
4. Logistic Regression
5. Voting Classifier

Considering the dataset's imbalance and prioritizing the accurate classification of the "Pathological" class, the following recommendation is made:

### Best Result

#### RandomOverSampler

#### Model: Random Forest

- Accuracy: 0.98
- F1-Score for Class 1 (Normal): 0.97
- F1-Score for Class 2 (Suspect): 0.97
- F1-Score for Class 3 (Pathological): 1.00

The Random Forest model with RandomOverSampler achieved the highest F1-Score (1.00) for the "Pathological" class, indicating the best performance in identifying high-risk cases. This makes it the recommended approach for this task.

## How to Use

To classify fetal health using this dataset, follow these steps:

1. Load the dataset.
2. Perform data preprocessing and exploration.
3. Implement RandomOverSampler or RandomUnderSampler to balance the classes.
4. Train one of the recommended models using the balanced dataset.
5. Evaluate the model's performance, with a focus on the "Pathological" class.

## Acknowledgements
Ayres de Campos et al. (2000) SisPorto 2.0 A Program for Automated Analysis of Cardiotocograms. J Matern Fetal Med 5:311-318 [link](https://onlinelibrary.wiley.com/doi/10.1002/1520-6661(200009/10)9:5%3C311::AID-MFM12%3E3.0.CO;2-9)
