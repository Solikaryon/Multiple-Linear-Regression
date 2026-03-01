# Multiple Linear Regression - Car Purchase Prediction

**Author:** Luis Fernando Monjaraz Briseño

## Project Description

This Jupyter notebook implements multiple linear regression using sklearn to predict car purchase amounts based on multiple features (annual salary and credit rating). The analysis demonstrates how to work with multiple independent variables to create a hyperplane prediction model.

## Dataset

The analysis uses the `car_purchasing.csv` dataset with the following key variables:
- **Independent Variables (X):** Annual Salary, Credit Rating
- **Dependent Variable (Y):** Car Purchase Amount

## Key Concepts

### Data Splitting
- **Training Set:** 70% of data
- **Test Set:** 30% of data

### Model Features

- Uses scikit-learn's `LinearRegression` class
- Creates a 3D hyperplane to visualize predictions
- Evaluates model performance using Mean Squared Error (MSE)
- Displays regression surface in 3D space

## Implementation Details

### Libraries Used
- `numpy` - Numerical computations
- `pandas` - Data manipulation
- `matplotlib` - Data visualization including 3D plotting
- `sklearn` - Machine learning models and metrics:
  - `LinearRegression` - Model training
  - `train_test_split` - Data partitioning
  - `mean_squared_error` - Model evaluation

### Model Coefficients

After training, the model provides:
- **Coefficients:** Weights for each independent variable
- **Intercept:** Base prediction value
- **Error Metrics:** MSE to evaluate model performance

## Visualizations

- **3D Scatter Plot:** Test data points in 3D space
- **Regression Surface:** Hyperplane showing model predictions
- **Data Visualization:** Blue dots represent actual test data
- **Model Representation:** Red surface represents the fitted hyperplane

## Mathematical Foundation

The multiple linear regression model follows:

$$\hat{y} = b_0 + b_1x_1 + b_2x_2$$

Where:
- $\hat{y}$ = predicted car purchase amount
- $b_0$ = intercept
- $b_1, b_2$ = coefficients for independent variables
- $x_1, x_2$ = annual salary and credit rating

## How to Run

1. Ensure Python 3.x is installed
2. Install required packages:
   ```bash
   pip install pandas numpy matplotlib scikit-learn
   ```
3. Place `car_purchasing.csv` in the same directory
4. Open and run the notebook:
   ```bash
   jupyter notebook "Multiple Linear Regression.ipynb"
   ```

## Model Evaluation

The notebook evaluates model performance using:
- **Mean Squared Error (MSE):** Average of squared differences between predicted and actual values
- Lower MSE values indicate better model fit

## Key Findings

- Multiple variables provide better predictions than simple linear regression
- The hyperplane visualization shows how the model predicts car purchase amounts
- Model performance is measured on unseen test data

## Technologies Used

- Python 3.x
- scikit-learn for machine learning
- Matplotlib for 3D visualization
- NumPy for numerical operations
- Pandas for data handling

## File Structure

```
.
├── Multiple Linear Regression.ipynb
├── car_purchasing.csv (required)
└── README.md
```

## Learning Objectives

This project demonstrates:
- Multiple linear regression theory
- Working with multiple independent variables
- 3D data visualization techniques
- Model evaluation and performance metrics
- Using scikit-learn for machine learning
- Train-test split methodology

## Notes

- Data is encoded in Latin-1
- Random state is set to 0 for reproducibility
- 3D visualization helps understand how the model works with multiple variables
