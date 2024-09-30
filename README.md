# car-price-lightgbm-catboost
Model training utilizing gradient boosting techniques, specifically leveraging LightGBM and CatBoost algorithms.
### README

# Car Price Prediction Model

## 1. Research Objective

The objective of this project is to analyze and predict the market value of a car based on its technical specifications, configurations, and the prices of similar vehicles. The following factors were considered in the model evaluation:

- **Prediction accuracy**: Measured using the RMSE (Root Mean Squared Error) metric.
- **Model training time**: Time taken to train each model.
- **Model prediction time**: Time taken to make predictions using each model.

## 2. Research Tasks

### 2.1 Data Loading and Exploration
- Load the dataset and perform initial exploration to understand the structure and content of the data.
- Clean the data by handling missing values, duplicates, and outliers.

### 2.2 Exploratory Data Analysis (EDA)
- Perform EDA to identify patterns, relationships, and distributions in the dataset.
- Analyze correlations between key features.

### 2.3 Data Preparation
- Prepare the dataset for machine learning by transforming and scaling features appropriately.
- Handle categorical and numerical features using techniques such as `OneHotEncoder` and `StandardScaler`.

### 2.4 Model Selection and Training
- Train multiple models including:
  - **Linear Regression**: A simple baseline model for comparison.
  - **Gradient Boosting Models**: LightGBM and CatBoost to leverage more sophisticated techniques.
  
### 2.5 Hyperparameter Tuning
- Tune hyperparameters of the models to optimize prediction performance.

### 2.6 Model Evaluation
- Evaluate the models based on the following criteria:
  - **Prediction quality**: Calculate the RMSE on the validation set.
  - **Training time**: Measure the time required to train each model.
  - **Prediction time**: Measure the time required to make predictions on the validation set.
  
- Compare all models and select the best one based on the combination of prediction accuracy, training time, and prediction time.

### 2.7 Test Set Evaluation
- After identifying the best model, run the final evaluation on the test set and report the performance metrics.

## 3. Data Source

- Dataset: `autos.csv`, containing data about cars, including technical specifications, configurations, and historical prices.

## 4. Project Structure

```
.
├── data/                  # Folder containing the dataset
├── notebooks/             # Jupyter notebooks for EDA and model development
├── src/                   # Python scripts for model training and evaluation
├── results/               # Folder to store model performance results
└── README.md              # This file
```

## 5. How to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/car-price-prediction.git
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Jupyter notebooks or Python scripts in the `src/` folder to train models and evaluate performance.

## 6. Conclusion

This project provides a thorough approach to predicting car prices using advanced machine learning techniques. The best-performing model was **LightGBM** with hyperparameters fine-tuned for optimal performance in terms of prediction accuracy and efficiency.

