# Dynamic Pricing Optimization for E-Commerce

## Overview
This project focuses on building a Dynamic Pricing Optimization model for an e-commerce platform. The model utilizes Support Vector Regression (SVR) to predict discounts based on relevant features such as customer care calls, customer rating, cost of the product, prior purchases, and weight in grams.

## Project Structure
- `ecommercedata.csv`: The dataset containing relevant information about an e-commerce site, we have used this dataset for training and testing the model.
- `Dynamic_Pricing_Ecommerce.ipynb`: Jupyter Notebook file with the Python code for data preprocessing, model training, hyperparameter tuning, and price optimization.

## Instructions
1. **Load Your Dataset:**
   - Load the dates into our jupiter notebook.

2. **Data Preprocessing:**
   - Adjust the features (`X`) and the target variable (`y`) based on your dataset structure.
   - Explore the relationships between features using a pairplot visualization.

3. **Train-Test Split:**
   - Split the data into training and testing sets.

4. **Feature Scaling:**
   - Standardize features using StandardScaler.

5. **Hyperparameter Tuning:**
   - Utilize Grid Search to find the best hyperparameters for the SVR model.

6. **Model Training:**
   - Train the SVR model with the best hyperparameters.

7. **Visualize Actual vs. Predicted Values:**
   - Use scatter plots to visualize the actual vs. predicted discount values.

8. **Check for Homoscedasticity:**
   - Examine the residual plot to assess homoscedasticity.

9. **Price Optimization:**
    - Provide new feature values to predict the discount for price optimization.

## Example Data for Price Optimization
You can use the provided example data in `new_data` for predicting discounts based on the trained model.

```python
# Example data for price optimization
new_data = pd.DataFrame({
    'Customer_care_calls': [3],
    'Customer_rating': [4],
    'Cost_of_the_Product': [80],
    'Prior_purchases': [2],
    'Weight_in_gms': [1500]
})
