# Heart-Disease-Prediction-Task
Build a model to predict whether a person is at risk of heart disease based on their health data.

# ---------------------------------------------------
Task Objective
# ---------------------------------------------------

The goal of this project is to predict whether a person is at risk of heart disease using machine learning. By analyzing clinical and physiological features such as age, sex, cholesterol, and maximum heart rate, the model can identify high-risk individuals. This project also highlights the key features that influence heart disease, providing insights for medical decision-making.

# ---------------------------------------------------
Dataset Used
# ---------------------------------------------------

Dataset Name: Heart Disease UCI Dataset

Source: Kaggle / UCI Machine Learning Repository

Features: 14 clinical features including:

age, sex, cp (chest pain type), trestbps (resting blood pressure), chol (serum cholesterol), fbs (fasting blood sugar), restecg (resting ECG results), thalach (maximum heart rate), exang (exercise-induced angina), oldpeak (ST depression), slope (slope of peak exercise ST segment), ca (number of major vessels colored by fluoroscopy), thal (thalassemia type)

Target Variable: condition (renamed to target) — indicates presence (1) or absence (0) of heart disease.

# ---------------------------------------------------
Major Steps in the Code
# ---------------------------------------------------
1. Dataset Loading and Preprocessing

The dataset is loaded using pandas.read_csv().

The label column condition is renamed to target for consistency.

Missing values are checked and handled if any.

Features are separated from the target variable.

Feature scaling is applied using StandardScaler to ensure all features are on the same scale for model training.

Data is split into training and testing sets (80% train, 20% test).

# ---------------------------------------------------
2. Exploratory Data Analysis (EDA)
# ---------------------------------------------------

Visualizations are used to understand the dataset:

Target Distribution: Shows the balance between patients with and without heart disease.

Correlation Heatmap: Highlights correlations between features and the target variable.

Pairplots: Visualizes relationships between numeric features and the target for better insight.

# ---------------------------------------------------
3. Model Training
# ---------------------------------------------------

A Logistic Regression model is trained on the scaled training set.

Logistic Regression is a baseline classifier suitable for binary outcomes.

The model learns the relationship between input features and the presence of heart disease.

# ---------------------------------------------------
4. Model Evaluation
# ---------------------------------------------------

Predictions are made on the test set.

Accuracy is calculated to measure overall performance.

Confusion Matrix shows true positives, true negatives, false positives, and false negatives.

Classification Report provides precision, recall, F1-score for each class.

ROC Curve and AUC: Evaluate the model’s ability to discriminate between classes; higher AUC indicates better performance.

# ---------------------------------------------------
5. Insights
# ---------------------------------------------------

Features such as thalach (max heart rate), cp (chest pain type), and oldpeak (ST depression) are highly influential for predicting heart disease.

Logistic Regression achieved an accuracy of ~XX% and an AUC of ~XX, indicating a strong baseline performance.

This workflow can be extended using more advanced classifiers like Decision Trees, Random Forests, or KNN for improved performance and feature importance analysis.

# ---------------------------------------------------
Models Applied
# ---------------------------------------------------

Logistic Regression: Baseline binary classification model.

(Optional extensions can include Decision Tree, Random Forest, KNN for comparison.)

# ---------------------------------------------------
Key Results and Findings
# ---------------------------------------------------

Logistic Regression accurately predicted heart disease presence/absence on the test set.

ROC-AUC score indicates strong discriminative ability.

Visualizations confirmed important features affecting prediction and revealed feature correlations.

Model insights can guide preventive measures and risk assessment in clinical settings.
