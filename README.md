# California Housing Prices Prediction

This project demonstrates how to use machine learning techniques to predict housing prices in California based on various features such as median income, house age, number of rooms, and more. The notebook walks through data loading, preprocessing, and training several models, evaluating their performance using RMSE.

## Project Structure

### 1. Data Loading and Exploration
- The dataset is loaded using the `pandas` library.
- Initial data exploration is conducted to understand the features and distributions.

### 2. Data Preprocessing
- Missing values are handled.
- Numerical features are scaled using `StandardScaler`.
- Categorical features are encoded using `OneHotEncoder`.
- A full preprocessing pipeline is constructed using `ColumnTransformer`.

### 3. Model Training
- Three models are trained and compared:
  - **Linear Regression**
  - **Decision Tree**
  - **Random Forest**
- The models are evaluated using RMSE (Root Mean Square Error) to compare their predictive performance.

### 4. Results
- The results are printed in the notebook after model evaluation:
  - **Linear Regression RMSE**: `68433.94`
  - **Decision Tree RMSE**: `0.0` (likely due to overfitting)
  - **Random Forest RMSE**: `18056.81`

## How to Run

1. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

2. Run the notebook:
    ```bash
    jupyter notebook 'Neural Networks - Project 1 California Housing Prices.ipynb'
    ```

3. The dataset used can be found [here](https://raw.githubusercontent.com/ageron/handson-ml/master/datasets/housing/housing.csv) (replace with your dataset source).

## Libraries Used

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`

## Improvements

- Fine-tune models to avoid overfitting in the Decision Tree.
- Try additional models like Gradient Boosting or XGBoost.
- Perform cross-validation to get a more reliable estimate of model performance.
