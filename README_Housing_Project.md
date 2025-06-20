
# 🏠 Housing Price Prediction with Machine Learning

This project aims to build a machine learning model that predicts housing prices in the Australian real estate market. It was developed for **Surprise Housing**, a US-based real estate company looking to expand into Australia.

## 📌 Project Objective

To develop a predictive model that accurately estimates house prices based on various property features, enabling informed investment decisions.

## 🔍 Problem Statement

Surprise Housing wants to use data science to:
- Strategically enter new markets
- Maximize revenue
- Optimize investment decisions

Given a dataset of housing attributes, the goal is to forecast sale prices and identify the most influential features that affect price.

## 🧾 Dataset

- **Train Dataset:** 1460 records, 81 features
- **Test Dataset:** Same format, no target column
- **Target Variable:** `SalePrice`
- **Features:** Both numerical and categorical (e.g., lot size, year built, neighborhood, etc.)

## 🧹 Data Preprocessing

- Handled missing values using domain-specific imputations
- Label encoding and one-hot encoding for categorical variables
- Standardization applied to numerical features

## 📊 Exploratory Data Analysis (EDA)

Used `seaborn` and `matplotlib` for:
- Distribution plots
- Heatmaps for correlation
- Boxplots to spot outliers
- Feature relationships with price

## 🏗️ Feature Engineering

- Created polynomial and interaction features
- Handled skewness in target and input variables
- Feature selection based on correlation and domain knowledge

## 🤖 Models Used

- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor

Each model was evaluated using:
- **Root Mean Squared Error (RMSE)**
- **Mean Squared Error (MSE)**
- **R² Score**

## 🧪 Hyperparameter Tuning

Used **GridSearchCV** with cross-validation to optimize parameters like:
- `alpha` for Ridge and Lasso
- `max_depth` and `n_estimators` for tree-based models

## ✅ Best Model

- **Ridge Regression** performed best after tuning.
- Final model was used to make predictions on the test dataset.
- Submission file created as `submission.csv`.

## 📈 Business Impact

- Helps Surprise Housing identify under- or overvalued properties.
- Enables strategic pricing and investment decisions based on data insights.

## 💼 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib
- Jupyter Notebook

## 📁 Project Structure

```
📦 Housing-Price-Prediction
│
├── housing_model.ipynb        # Jupyter Notebook with full pipeline
├── train.csv                  # Training dataset
├── test.csv                   # Test dataset
├── submission.csv             # Final predictions
├── requirements.txt           # Python dependencies
├── README.md                  # Project documentation
└── .gitignore                 # Git ignore rules
```

## 📌 Future Work

- Try XGBoost and LightGBM for performance boost
- Add geolocation-based features
- Deploy as a web app using Streamlit or Flask

## 🙌 Acknowledgements

Thanks to the Surprise Housing team for the data and opportunity to apply predictive modeling to real estate!

## 📫 Contact

Feel free to reach out via [GitHub Issues](https://github.com/your-username/your-repo-name/issues) for feedback or questions.
