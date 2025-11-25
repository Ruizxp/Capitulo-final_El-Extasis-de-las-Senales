# Biosignals Processing
## Proyecto 3: Statistical Analysis of Respiratory Audio to Differentiate Healthy Patients, Patients with Wheezing, and Patients with Crackles

This project analyzes a respiratory audio dataset to determine whether statistically significant differences exist among healthy individuals, patients with wheezing, and patients with crackles. The workflow includes:

## Data Preprocessing

- Filtering: High-pass and low-pass filters are applied to clean the recordings and remove unwanted noise.

- Wavelet Decomposition: Wavelet-based denoising is used to reduce cardiac rhythm artifacts present in the respiratory signals.

## Statistical Analysis

- Assumption Checks: Normality and homoscedasticity are evaluated to determine the suitability of parametric tests.

- Parametric Testing: Parametric tests are attempted; however, the homogeneity of variances assumption is not satisfied.

- Non-Parametric Testing: Due to the violation of assumptions, a non-parametric Mann–Whitney U test is conducted.

## Results

- Statistically significant differences are found across all combinations of patient groups.

- Non-parametric methods successfully capture the differences between groups when parametric methods are not applicable.

## Key Findings

- Clear statistical differences exist between wheezing patients and healthy individuals.

- Non-parametric approaches offer robust conclusions when assumptions of classical methods are not met.

## Proyecto 4: Classification of Patient Respiratory Audio Using Machine Learning and Deep Learning Techniques

In this project machine learning (SVM machines and k-means)and deep learning (CNN) models are implemented to classify respiratory audio recordings into clinical categories (healthy, wheezing, and crackles). The goal is to evaluate and compare different approaches for respiratory sound classification.
Performance is assessed using accuracy, F1-score, confusion matrices, and cross-validation strategies.

## Results

- Increasing the training data consistently reduced log-loss and narrowed the gap between training and validation scores, suggesting that more data would improve model stability and reduce overfitting, especially in the three-class problem.

- The 200–280 Hz PSD differences helped distinguish wheezing cycles in binary comparisons, but this feature showed weak correlation overall, indicating that additional features are needed for more robust classification.

- Model performance did not scale with complexity, and both clustering (K-means) and SVC showed poor multi-class separation due to strong overlap in the feature space, with SVC achieving high accuracy only for healthy cycles at the expense of the other classes.
