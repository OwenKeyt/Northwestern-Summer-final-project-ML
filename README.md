## About The Project

This project predicts a student's chance of admission to graduate school based on their academic profile. It uses a dataset from Kaggle and compares three different regression models to evaluate their performance.

**Project Origin:** This was my final project for an introductory machine learning course I completed at Northwestern University during the summer after my sophomore year of high school.

## Methodology

The project follows a standard machine learning workflow:
1.  **Data Cleaning & EDA:** The dataset was loaded, inspected for null values, and visually analyzed using histograms and boxplots to understand data distributions.
2.  **Outlier Removal:** Two outliers were identified and removed from the "Chance of Admit" variable using the Interquartile Range (IQR) method to reduce skew.
3.  **Modeling:** Three different regression models were trained and tested:
    * Linear Regression
    * Polynomial Regression (Degree 2)
    * Random Forest Regressor
4.  **Evaluation:** Models were evaluated using the R² score and by plotting the distribution of the residuals.

## Results

The models performed as follows on the test data:
* **Linear Regression:** R² = 0.79
* **Polynomial Regression:** R² = 0.77
* **Random Forest:** R² = 0.74

The Linear Regression model provided the best fit for this particular dataset.

## Retrospective & Future Improvements

Looking back on this project from a few years ago, I would now implement a few additional steps to improve it:
* **Feature Scaling:** Look in to using a standard scalar to scale all numerical features before fitting the models.
* **Hyperparameter Tuning:** Using more tools on the Random Forest model to find the optimal hyperparameters.
* **Additional Metrics:** Evaluate the models using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) in addition to R².
