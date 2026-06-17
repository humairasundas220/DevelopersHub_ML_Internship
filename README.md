# DevelopersHub_ML_Internship
# AI/ML Engineering Internship Tasks — DevelopersHub Corporation

## Task 1: Exploring and Visualizing the Iris Dataset

### Task Objective
Load, inspect, and visualize the Iris dataset to understand
data trends, distributions, and relationships between features.

### Dataset Used
- **Name:** Iris Dataset
- **Source:** Loaded via seaborn, saved as CSV using pandas
- **Size:** 150 samples, 4 features, 3 classes

### Models Applied
No model applied — this is an EDA (Exploratory Data Analysis) task.

### Key Results and Findings
1. Dataset has 150 samples, 3 balanced classes, no missing values.
2. Petal length & width best separate the 3 species visually.
3. Iris Setosa is clearly separable from Versicolor and Virginica.
4. A few outliers exist in sepal_width for Setosa (visible in box plots).
5. Petal features are the most useful for future classification tasks.

## Task 2: Predict Future Stock Prices (Short-Term)

### Task Objective
Use historical stock data to predict the next day's closing price 
using features like Open, High, Low, and Volume.

### Dataset Used
- **Name:** AAPL (Apple Inc.) historical stock data
- **Source:** Yahoo Finance, fetched via the `yfinance` Python library
- **Period:** January 2022 – June 2026
- **Size:** 1117 trading days, 4 features (Open, High, Low, Volume)

### Models Applied
- Linear Regression

### Key Results and Findings
- MAE: 3.21 → predictions are off by ~$3.21 on average
- RMSE: 4.39 → indicates a few larger errors exist
- High and Low prices were the most influential features
- Volume had negligible impact on prediction due to scale difference
- The model's predictions closely tracked actual closing price trends,
  showing strong performance relative to AAPL's price range (~$150-200)

## Task 3: Heart Disease Prediction

### Task Objective
Build a classification model to predict whether a person is at risk 
of heart disease based on their health data.

### Dataset Used
- **Name:** Heart Disease UCI Dataset
- **Source:** Kaggle / UCI Machine Learning Repository
- **Size:** 302 patient records (after removing 1 duplicate), 13 features + target

### Models Applied
- Logistic Regression

### Key Results and Findings
- Accuracy: 79%
- AUC Score: 0.86
- Recall for Disease class: 88% (model catches most actual disease cases)
- Most influential features: chest pain type (cp), sex, max heart rate 
  (thalach), and ST depression (oldpeak)
- Age and fasting blood sugar had minimal influence, contrary to common 
  assumptions about age being a dominant risk factor
