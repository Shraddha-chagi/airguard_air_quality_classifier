# AirGuard: Explainable Air-Pollution Classification

## Project Overview

AirGuard is a beginner-friendly machine learning project that classifies observed carbon monoxide (CO) concentration into lower, moderate, and higher relative categories using environmental and gas-sensor measurements.

The project compares a Decision Tree classifier with a K-Nearest Neighbors (KNN) classifier and investigates which features contribute most to the Decision Tree's predictions.

**Note:** The categories are based on the dataset's CO concentration distribution. They are not official AQI categories or medical safety recommendations.

## Dataset

- **Source:** [UCI Machine Learning Repository — Air Quality](https://archive.ics.uci.edu/dataset/360/air+quality)
- **Observations:** 9,358 hourly records in the original dataset
- **Features:** Gas-sensor readings, pollutant measurements, temperature, and humidity
- **Target:** Three relative CO concentration classes

## Technologies

- Python
- pandas and NumPy
- Matplotlib
- scikit-learn
- Google Colab / Jupyter Notebook

## Models

1. Decision Tree Classifier
2. K-Nearest Neighbors (KNN)

## Evaluation

Both models are evaluated on the same held-out test set using accuracy, a classification report, and a confusion matrix.

- Decision Tree accuracy: 84.23%
- KNN accuracy: 86.12%
- Better-performing model: K-Nearest Neighbors (KNN)

## How to Run

1. Open `airguard_air_quality_classifier.ipynb` in Google Colab or Jupyter Notebook.
2. Run the notebook cells from top to bottom.
3. The notebook downloads the dataset and performs preprocessing, training, and evaluation.

## Conclusion

AirGuard compared two machine learning models, Decision Tree and K-Nearest Neighbors (KNN), to classify observed CO concentrations into lower, moderate, and higher relative categories using the UCI Air Quality dataset.

KNN achieved an accuracy of **86.12%**, outperforming the Decision Tree, which achieved **84.23%**, by approximately 1.89 percentage points. The Decision Tree's feature-importance analysis identified `PT08.S2(NMHC)` as the most influential feature (72.48%), followed by `NOx(GT)` (16.41%).

The confusion matrices helped evaluate classification errors across the three categories. This project provided practical experience in data cleaning, handling missing values, feature preparation, model training, evaluation, and feature-importance analysis.

AirGuard is an educational classification prototype, not a real-time pollution forecasting system or an official air-quality warning tool. Future improvements could include more rigorous validation, testing on independent datasets, and further analysis of class-wise precision and recall.

## Limitations

AirGuard classifies observed CO concentration categories rather than predicting future pollution or official air-quality alerts. The dataset comes from a historical monitoring location in Italy, so its results should not automatically be generalized to other locations.

## Dataset Citation

Vito, S. (2008). Air Quality. UCI Machine Learning Repository. https://doi.org/10.24432/C59K5F
