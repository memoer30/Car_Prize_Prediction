# Car Price Prediction using Regression

A machine learning project that predicts car prices using various regression algorithms. This project demonstrates data preprocessing, handling missing values, feature engineering, model comparison, and hyperparameter tuning.

## 📋 Project Overview

This project uses scikit-learn to build and compare multiple regression models for predicting car sale prices. The dataset contains car features including make, color, odometer reading, and number of doors, with some missing values that are handled through preprocessing pipelines.

## 🎯 Features

- **Data Preprocessing**: Complete pipeline using scikit-learn's `ColumnTransformer` and `Pipeline`
- **Missing Value Handling**: Intelligent imputation strategies for both categorical and numerical features
- **Feature Engineering**: One-hot encoding for categorical variables
- **Multiple Models**: Comparison of Ridge, Random Forest, Gradient Boosting, and XGBoost regressors
- **Hyperparameter Tuning**: GridSearchCV optimization for best model performance
- **Comprehensive Evaluation**: R² score, Mean Absolute Error (MAE), and Mean Squared Error (MSE) metrics

## 📊 Dataset

The dataset (`car-sales-extended-missing-data.csv`) contains the following features:

- **Make**: Car manufacturer (Honda, BMW, Toyota, Nissan)
- **Colour**: Car color
- **Odometer (KM)**: Distance traveled in kilometers
- **Doors**: Number of doors
- **Price**: Sale price (target variable)

**Note**: The dataset contains missing values which are handled during preprocessing.

## 🛠️ Technologies Used

- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **scikit-learn**: Machine learning algorithms and preprocessing
- **XGBoost**: Advanced gradient boosting implementation
- **Matplotlib**: Data visualization

## 📦 Installation

1. Clone this repository:
```bash
git clone git@github.com:memoer30/Car_Prize_Prediction.git
cd Car_Prize_Prediction_Regresion
```

2. Install required packages:
```bash
pip install pandas numpy scikit-learn xgboost matplotlib jupyter
```

## 🚀 Usage

1. Open the Jupyter notebook:
```bash
jupyter notebook Car_Prize_Prediction_Regresion.ipynb
```

2. Run all cells to:
   - Load and explore the data
   - Build preprocessing pipelines
   - Train multiple regression models
   - Compare model performance
   - Perform hyperparameter tuning

## 🔍 Methodology

### 1. Data Preprocessing

- **Categorical Features** (Make, Colour):
  - Missing values filled with "missing"
  - One-hot encoded for model compatibility

- **Numerical Features** (Odometer):
  - Missing values imputed with mean strategy

- **Doors Feature**:
  - Missing values filled with constant value (4)
  - Treated as numerical feature

### 2. Models Implemented

| Model | Description |
|-------|-------------|
| **Ridge Regression** | Linear regression with L2 regularization |
| **Random Forest** | Ensemble of decision trees |
| **Gradient Boosting** | Sequential boosting algorithm |
| **XGBoost** | Optimized gradient boosting |

### 3. Model Evaluation

Models are evaluated using:
- **R² Score**: Coefficient of determination (0 to 1, higher is better)
- **Mean Absolute Error (MAE)**: Average absolute difference between predictions and actual values
- **Mean Squared Error (MSE)**: Average squared difference (penalizes larger errors more)

### 4. Hyperparameter Tuning

GridSearchCV is used to optimize:
- Random Forest: `n_estimators`, `max_depth`, `min_samples_split`
- Gradient Boosting: `learning_rate`, `n_estimators`, `max_depth`, `subsample`

## 📈 Results

The notebook compares all models and identifies the best performing algorithm through:
- Cross-validation scores
- Test set performance
- Optimized hyperparameters

## 📁 Project Structure

```
Car_Prize_Prediction_Regresion/
│
├── Car_Prize_Prediction_Regresion.ipynb   # Main Jupyter notebook
├── README.md                              # Project documentation
```

## 🔑 Key Learnings

- Building end-to-end machine learning pipelines
- Handling real-world messy data with missing values
- Comparing multiple regression algorithms
- Hyperparameter optimization techniques
- Feature engineering for categorical data
- Model evaluation and selection

## 🤝 Contributing

Feel free to fork this project and submit pull requests for any improvements.

## 📝 License

This project is open source and available for educational purposes.

## 👤 Author

Created as a machine learning practice project demonstrating regression techniques and scikit-learn pipelines.

---

**Note**: This is an educational project demonstrating machine learning regression techniques with scikit-learn.
