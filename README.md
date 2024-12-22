# Prediction-using-Supervised-ML

This repository contains a Python notebook (`Prediction using Supervised ML.ipynb`) that implements a simple linear regression model to predict student scores based on the number of hours they studied. The model uses the Scikit-learn library for training and evaluation.

## Dataset

The dataset used in this project contains two columns: 'Hours' (the number of hours studied) and 'Scores' (the corresponding percentage score). The data is loaded from a remote CSV file using the provided URL `http://bit.ly/w-data`. This is a simple dataset with 25 records to show a simple linear regression model.

## Code Overview

The Python notebook (`Prediction using Supervised ML.ipynb`) includes the following steps:

1.  **Import Libraries:** Imports required libraries such as `pandas` for data manipulation, `numpy` for numerical operations, `matplotlib.pyplot` for data visualization, and  `sklearn` for building the regression model.
2.  **Load Data:** Loads the dataset into a pandas DataFrame from the provided URL.
3.  **Data Exploration:**
    -   Displays the first few rows of the DataFrame (`head()`).
    -   Shows information about the DataFrame's columns and data types (`info()`).
    -   Generates descriptive statistics (`describe()`).
    -   Creates a scatter plot to visualize the relationship between 'Hours' and 'Scores'.
4.  **Data Preparation:**
    -   Splits the data into 'attributes' (input features, 'Hours') and 'labels' (target variable, 'Scores').
    -   Divide the data into training and testing sets using `train_test_split` (80% for training and 20% for testing).
5.  **Model Training:**
    -   Creates an instance of the `LinearRegression` model.
    -   Trains the model using the training data (`fit()`).
6.  **Regression Line Visualization:**
    -   Calculates the regression line using the model’s coefficients and intercept.
    -   Plots the data points and the regression line on the same graph.
7.  **Prediction:**
    -   Predicts the scores for the test data (`predict()`).
    -   Displays both the actual and predicted scores as a table for comparison.
8.  **Model Evaluation:**
    -   Predicts the score of students if study for 9.25 hours.
    -   Calculates the Mean Absolute Error.
    -   Calculates the R-squared value to asses the model performance.

## Key Findings

The notebook shows that:

*   There is a positive linear relationship between the number of hours studied and the percentage score achieved.
*   The linear regression model provides an r-squared of 0.945 and MAE of 4.18.

## How to Run

1.  Clone the repository to your local machine.
2.  Ensure you have the necessary Python libraries installed (`pandas`, `numpy`, `matplotlib`, `scikit-learn`). If not, install them using `pip install pandas numpy matplotlib scikit-learn`.
3.  Open `Prediction using Supervised ML.ipynb` using Jupyter Notebook or JupyterLab.
4.  Run the notebook cells sequentially to see the results.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
