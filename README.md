# Stroke Prediction on Imbalanced Dataset

A project to predict stroke from patient data using various machine learning approaches on a highly imbalanced dataset (98% non-stroke, 2% stroke).

## Overview
This project addresses the challenge of classifying rare stroke cases in an extremely imbalanced dataset. Multiple techniques were explored, including one-class classification, undersampling, clustering-based sampling, and threshold tuning, to improve model performance on the minority class.

## Dataset
- Highly imbalanced dataset with 98% non-stroke and 2% stroke cases
- Source: https://www.kaggle.com/datasets/shashwatwork/cerebral-stroke-predictionimbalaced-dataset

## Methods Explored
1. **One-Class Classification with Autoencoders**  
   Treating stroke as anomalies to detect rare events.

2. **Undersampling Techniques**  
   - Tomek Links  
   - Edited Nearest Neighbors (ENN)
   - Condensed Nearest Neighbors (CNN)

3. **Clustering-Based Undersampling**  
   Remove a percentage of majority class points per cluster to preserve data distribution.

4. **Threshold Tuning**  
   Adjusting probability thresholds to optimize F1-score for minority class.

## Results
- Baseline F1-score for stroke: **0.07**  
- After applying above techniques: **0.113**  
- The small improvement reflects the extreme imbalance and difficulty of detecting rare events.

## License
This project is for educational purposes only. Contact the author for reuse or commercial purposes.
