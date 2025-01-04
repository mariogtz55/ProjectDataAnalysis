# Customer Conversion Prediction

## Project Purpose

This project aims to build a model that predicts customer conversion using a dataset from JARSA. This prediction can help JARSA anticipate which customers are more likely to convert and allocate resources accordingly, improving sales and customer relationship management.

## Methodology

1. **Data Loading and Preprocessing:**
    - Data was loaded from an Excel file ('datos_jarsa3.xlsx') and a SPSS file ('JARSA.sav') using the pandas library.
    - The data was cleaned and preprocessed:
        - Irrelevant columns and rows were removed.
        - Missing values were handled.
        - Categorical features were converted to numerical using one-hot encoding.

2. **Exploratory Data Analysis:**
    - The data was explored to understand relationships between variables:
        - Grouped data to identify patterns and trends.
        - Created visualizations using `matplotlib.pyplot` and `seaborn` to visualize sales and customer behaviour.

3. **Feature Selection:**
    -  Two approaches were used for feature selection to improve model performance and reduce model complexity:
        - Feature importance from logistic regression coefficients
        - Identifying features with the highest and lowest correlation with customer conversion  

4. **Model Building and Evaluation:**
    - Two models were built:
        - **Logistic Regression:** To predict the probability of customer conversion (win or loss).
        - **Linear Regression:** To try and predict the discrete customer conversion state.
    - The models were trained and evaluated using metrics such as accuracy, precision, recall, and F1-score.
    - Standard scaling was used to improve model performance

## Results

- The Logistic Regression model showed promising results in predicting customer conversion, with reasonable accuracy, precision, recall, and F1-score.
- Linear Regression was not able to make good discrete predictions on the outcome variable, but model coefficients may provide data insights.
- The model coefficients were analyzed to understand which features were most influential in customer conversion prediction.


## Conclusion

This project provides a foundation for predicting customer conversion at JARSA. The built models can be further refined and deployed to improve decision-making in sales and customer management.
