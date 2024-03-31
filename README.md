# House Prices Prediction - Advanced Regression

This project aims to predict house prices using advanced regression techniques. The dataset used for this project is from a Kaggle competition titled "House Prices: Advanced Regression Techniques".

## Dataset
The dataset contains various features describing different aspects of residential homes in Ames, Iowa. These features include information such as the size of the house, its condition, location, and many others. The target variable is the sale price of the houses.

## Approach
The project follows a standard machine learning pipeline:

1. **Data Importing and Preprocessing**: The dataset is imported, missing values are handled, and categorical variables are encoded. The data is then split into training and validation sets.

2. **Model Training and Evaluation**: Several regression models are trained and evaluated using the training and validation datasets. Models include Random Forest, AdaBoost, and XGBoost. Hyperparameter tuning is performed for XGBoost using Grid Search CV to improve performance.

3. **Prediction and Submission**: The best performing model (XGBoost) is used to predict house prices on the test dataset. The predictions are saved in a submission file for the Kaggle competition.

## Model Performance
- Random Forest Validation RMSE: 28,813.73
- AdaBoost Validation RMSE: 36,359.11
- XGBoost Validation RMSE (Before Hyperparameter Tuning): 25,888.99
- XGBoost Validation RMSE (After Hyperparameter Tuning): 24,695.46

## Kaggle Submission Score
The submission achieved a Kaggle score of 0.13869.

## Files
- `submission.csv`: Contains the predictions made on the test dataset for submission to the Kaggle competition.
- `house_price_prediction.ipynb`: Jupyter notebook containing the complete code for data preprocessing, model training, and evaluation.

## Dependencies
- Python 3.x
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost

## How to Use
1. Clone the repository.
2. Install the required dependencies.
3. Run the Jupyter notebook `house_price_prediction.ipynb` to replicate the analysis and predictions.

## Note
Ensure that the paths to the dataset files are correctly specified if running the code on your local machine.

