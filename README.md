# Cardiovascular Disease Analysis Using Deep Learning


## Project Overview

This project focuses on predicting the presence of heart disease using a Deep Learning-based Artificial Neural Network (ANN) implemented in PyTorch. The objective is to build a binary classification model that can determine whether a patient is likely to have heart disease based on various clinical attributes.

The project includes Exploratory Data Analysis (EDA), data preprocessing, model development, training, evaluation, and performance analysis.

## Dataset Information

The dataset contains clinical and medical attributes related to heart disease prediction.

### Features

* Age
* Sex
* Chest Pain Type (cp)
* Resting Blood Pressure (trestbps)
* Cholesterol (chol)
* Fasting Blood Sugar (fbs)
* Resting ECG Results (restecg)
* Maximum Heart Rate Achieved (thalach)
* Exercise Induced Angina (exang)
* ST Depression (oldpeak)
* Slope of Peak Exercise ST Segment (slope)
* Number of Major Vessels (ca)
* Thalassemia (thal)

### Target Variable

* 0 = No Heart Disease/Cardiovascular Disease
* 1 = Heart Disease/ Cardiovascular Disease

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* PyTorch

## Exploratory Data Analysis (EDA)

The following analyses were performed:

* Dataset inspection
* Statistical summary
* Target variable distribution
* Correlation analysis
* Heatmap visualization
* Feature relationship analysis
* Boxplots and distribution plots
* Outlier detection
* Missing value analysis

## Data Preprocessing

The following preprocessing steps were applied:

1. Data loading
2. Removal of unnecessary columns
3. Feature scaling using StandardScaler
4. Train-test split (80:20)
5. Conversion of data into PyTorch tensors

## Deep Learning Model Architecture

The Artificial Neural Network (ANN) consists of:

Input Layer

→ Dense Layer (128 neurons)

→ ReLU Activation

→ Batch Normalization

→ Dropout (0.30)

→ Dense Layer (64 neurons)

→ ReLU Activation

→ Batch Normalization

→ Dropout (0.30)

→ Dense Layer (32 neurons)

→ ReLU Activation

→ Dropout (0.20)

→ Output Layer (1 neuron)

## Training Configuration

| Parameter        | Value             |
| ---------------- | ----------------- |
| Optimizer        | Adam              |
| Learning Rate    | 0.0005            |
| Loss Function    | BCEWithLogitsLoss |
| Epochs           | 100               |
| Batch Size       | 16                |
| Train-Test Split | 80:20             |

## Model Performance

### Classification Report

| Metric    | Class 0 | Class 1 |
| --------- | ------- | ------- |
| Precision | 0.77    | 0.77    |
| Recall    | 0.71    | 0.82    |
| F1-Score  | 0.74    | 0.79    |

### Overall Accuracy

**Accuracy = 77.05%**

The model correctly predicts approximately 77 out of every 100 patients.

## Confusion Matrix

| Actual / Predicted | No Heart Disease | Heart Disease |
| ------------------ | ---------------- | ------------- |
| No Heart Disease   | 20               | 8             |
| Heart Disease      | 6                | 27            |

### Interpretation

* True Negatives (TN) = 20
* False Positives (FP) = 8
* False Negatives (FN) = 6
* True Positives (TP) = 27

The model successfully identified most heart disease cases while maintaining balanced classification performance.

## Conclusion

A Deep Learning-based Artificial Neural Network (ANN) was successfully developed for heart disease prediction. The model achieved an overall accuracy of 77.05% and demonstrated strong recall (82%) for detecting heart disease cases. These results indicate that Deep Learning can effectively classify cardiovascular disease risk using clinical patient attributes.

Future improvements may include:

* Hyperparameter tuning
* Feature engineering
* Cross-validation
* Ensemble learning methods
* Comparison with Machine Learning algorithms such as Random Forest and XGBoost
  
## Author

Heart Disease Prediction Using Deep Learning Project

Developed using Python, Scikit-Learn, and PyTorch.
