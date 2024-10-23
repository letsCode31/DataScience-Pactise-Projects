# Titanic Dataset - Exploratory Data Analysis (EDA)

This project performs exploratory data analysis on the Titanic dataset to understand the data, clean it, and visualize various patterns. The aim is to uncover insights that can help predict the survival of passengers based on features like age, gender, class, and fare.

## Project Overview
The Titanic dataset contains information about passengers who were on the Titanic. This analysis aims to explore the dataset, perform data cleaning, visualize key features, and understand the relationships between different variables.

### Steps Involved
1. **Data Loading**: Load the dataset from Seaborn's built-in datasets.
2. **Data Cleaning**:
   - Fill missing values for `age` based on gender-specific median values.
   - Fill missing values for `embarked` using the most common value.
   - Drop columns with too many missing values (`deck`, `embark_town`).
3. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of ages.
   - Analyze survival rate by gender and passenger class.
   - Generate a correlation heatmap for selected features (`age`, `sex`, `survived`, `pclass`, and `fare`).
   - Create a scatter plot between `age` and `fare`.
   - Plot a boxplot to understand age distribution across different passenger classes and genders.

## Requirements
Make sure to have the following Python libraries installed:
- `pandas`
- `seaborn`
- `matplotlib`

You can install these using:
```bash
pip install pandas seaborn matplotlib
