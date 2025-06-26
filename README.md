# Digit-Recognizer
This project was completed as part of **STA 160: Practice in Statistical Data Science** at UC Davis. It explores how low-dimensional, interpretable features can be used to classify handwritten digits from the MNIST dataset — without relying on deep learning and raw pixel analysis.

## Project Objective
The goal was to apply practical statistical data science skills to a real-world classification task. By creating and evaluating simple yet meaningful features, the project demonstrates how far basic statistical intuition can go in understanding and classifying digit images.

## Dataset
- **Source**: MNIST Handwritten Digits Kaggle Competition Dataset  
- **Structure**: 28×28 grayscale images with 10,000+ data

## Feature Engineering
Six features were extracted from the raw pixel matrix:
- `total_ink`: Total sum of pixel intensities  
- `avg_intensity`: Average pixel intensity  
- `std_intensity`: Standard deviation of pixel values  
- `active_pixels`: Count of nonzero pixels  
- `min_nonzero_intensity`: Minimum intensity among active pixels  
- `max_intensity`: Maximum pixel intensity

## Methodology
- Exploratory Data Analysis (EDA) to investigate digit complexity
- t-SNE for dimensionality reduction and cluster visualization
- Applied and compared multiple classifiers:
  - K-Nearest Neighbors (KNN)
  - Random Forest
  - Gradient Boosting

## Key Findings
- Gradient Boosting achieved the highest accuracy (~29%)  
- Certain digits (like 1 and 7) are easier to distinguish based on ink patterns  
- Even with limited features, models captured meaningful variance in digit identity

## Language & Library Used
- Python (NumPy, Pandas, Matplotlib, Seaborn)
- scikit-learn
- t-SNE for visualization

## Reflection
This project emphasized the power of interpretable feature engineering and practical statistical modeling. It reinforced my belief that data science isn’t always about complex models — sometimes, simple insights go a long way, especially in high-stakes domains like finance or automation.
