The goal of this project is to build a predictive model that estimates the sale price of a house based on various features such as the overall quality, living area, garage capacity, year built, and number of bathrooms. We use a simple linear regression algorithm to achieve this and evaluate the model's performance with real-world data.

## Dataset

I used the **Ames Housing Dataset**, which is a popular dataset for regression tasks related to house price prediction. The dataset consists of various features describing different aspects of houses, such as:

- **OverallQual**: Overall material and finish quality
- **GrLivArea**: Above-ground living area in square feet
- **GarageCars**: Size of the garage in terms of car capacity
- **YearBuilt**: Year the house was built
- **FullBath**: Number of full bathrooms above ground

The target variable is `SalePrice`, which represents the price of the house.

## Steps Involved

1. **Data Loading and Exploration**
   - Load the dataset using `fetch_openml` from scikit-learn.
   - Explore the dataset and check for missing values.

2. **Data Preparation**
   - Select key features and the target variable.
   - Split the dataset into training and testing sets.

3. **Model Training**
   - Train a linear regression model using the training set.
   - Make predictions on the testing set.

4. **Model Evaluation**
   - Evaluate the model's performance using metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² score.

5. **Visualization**
   - Plot the correlation matrix to understand feature relationships.
   - Visualize scatter plots of actual vs. predicted house prices.
