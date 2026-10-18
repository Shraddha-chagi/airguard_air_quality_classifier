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

- Decision Tree accuracy: [Fill in actual result]
- KNN accuracy: [Fill in actual result]
- Better-performing model: [Fill in after evaluation]

## How to Run

1. Open `airguard_air_quality_classifier.ipynb` in Google Colab or Jupyter Notebook.
2. Run the notebook cells from top to bottom.
3. The notebook downloads the dataset and performs preprocessing, training, and evaluation.

## Conclusion

[Write your conclusion after running both models. Compare their actual test results, discuss classification errors, and describe the most important features identified by the Decision Tree.]

## Limitations

AirGuard classifies observed CO concentration categories rather than predicting future pollution or official air-quality alerts. The dataset comes from a historical monitoring location in Italy, so its results should not automatically be generalized to other locations.

## Dataset Citation

Vito, S. (2008). Air Quality. UCI Machine Learning Repository. https://doi.org/10.24432/C59K5F
