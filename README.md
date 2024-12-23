# Sales Forecasting Project

## Project Overview
This project aims to forecast product sales quantities using machine learning techniques. The dataset includes historical sales records, weather conditions, product categories, and other contextual data. The project leverages advanced feature engineering and ensemble learning methods to deliver accurate predictions.

## Features and Techniques
- **Data Cleaning**: Removing missing values to ensure data integrity.
- **Feature Engineering**:
  - Temporal features: Year, month, day, day of the week, and quarter.
  - Additional insights: Weekend flag, seasonality categorization, and weather-region interactions.
- **Categorical Encoding**: One-hot encoding for categorical variables.
- **Feature Scaling**: StandardScaler used to normalize features.
- **Model Training**:
  - Random Forest Regressor with hyperparameter optimization (RandomizedSearchCV).
  - Gradient Boosting Regressor and AdaBoost Regressor.
  - Ensemble model (Voting Regressor) combining the above models.
- **Performance Metric**: Mean Absolute Percentage Error (MAPE).

## Dataset Description
- **Training Data**: Contains sales records with features such as date, product category, brand, weather conditions, and sales quantity.
- **Submission Data**: Test data for which sales quantities need to be predicted.

## Project Files
- `train.csv`: Training dataset.
- `submission.csv`: Template for submission with product IDs and predicted quantities.
- `DataTour.ipynb`: Python script containing the complete implementation.
- `submission.csv`: Final submission file with predictions.

## Prerequisites
Ensure the following libraries are installed in your Python environment:
```bash
pip install pandas numpy scikit-learn
```

## Usage
1. Clone the repository and navigate to the project directory.
2. The output `submission.csv` file will contain the predicted sales quantities.

## Key Results
- **MAPE**: The ensemble learning model achieved a MAPE score of `{:.2f}` on the test dataset.
- **Top Features**:
  The model identified the following as the most important features:
  - Year
  - Month
  - Weather-region interactions
  - Product brand and category

## Future Work
- Include additional data sources to improve model performance.
- Experiment with deep learning techniques for time-series analysis.
- Build a web interface for real-time sales predictions.

## Contact
For inquiries, reach out to [yonlifidelis2@gmail.com].
