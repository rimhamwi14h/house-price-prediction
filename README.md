# House Price Prediction

Machine Learning project to predict house prices using Python and scikit-learn.

## Project Overview

The objective of this project is to build a regression model capable of predicting house prices based on different property characteristics.

The project includes data exploration, preprocessing, model training, evaluation and model comparison.

## Dataset

The project uses the Ames Housing dataset.

- 1460 houses
- 80 input features
- Target: `SalePrice`

The dataset contains numerical and categorical variables.

## Data Preprocessing

The preprocessing pipeline includes:

- Missing numerical values replaced with the median
- Missing categorical values replaced with the most frequent value
- One-Hot Encoding for categorical variables
- Train/Test split: 80% training and 20% testing

## Models

Two regression models were tested:

- Linear Regression
- Random Forest Regressor

## Results

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 20548.77 | 31269.66 | 0.8725 |
| Random Forest | 17487.10 | 28348.44 | 0.8952 |

Random Forest achieved better performance on the test set.

## Feature Importance

Some of the most important features identified by the Random Forest model were:

- OverallQual
- GrLivArea
- TotalBsmtSF
- 2ndFlrSF
- 1stFlrSF

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- scikit-learn
- Jupyter Notebook
- Joblib
- Git
- GitHub

## Project Structure

```text
house-price-prediction/
│
├── models/
│   └── house_price_model.pkl
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   └── 02_preprocessing_and_model.ipynb
│
├── .gitignore
├── README.md
└── requirements.txt