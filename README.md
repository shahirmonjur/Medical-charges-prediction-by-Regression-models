## Problem Statement

> ACME Insurance Inc. offers affordable health insurance to thousands of customer all over the United States. 

> This is primarily a data analysis and feature analysis notebook that also trains regression models to predict the medical charges of a customer of the insurance company given their data like age, BMI, how many children they have.
>
> Estimates from this system will be used to determine the annual insurance premium (amount paid every month) offered to the customer. Due to regulatory requirements, the insurance company must be able to explain why their system outputs a certain prediction.
>
> We have found a [CSV file](https://raw.githubusercontent.com/JovianML/opendatasets/master/data/medical-charges.csv) containing verified historical data, consisting of the aforementioned information and the actual medical charges incurred by over 1300 customers.
> 
> <img src="https://i.imgur.com/87Uw0aG.png" width="480">
>
> Dataset source: https://github.com/stedy/Machine-Learning-with-R-datasets

## Dataset Description
> The dataset contains information about 1,338 customers, including their age, sex, BMI, number of children, smoking habits, region of residence, and annual medical charges. For this project, we focus on non-smokers and use their age and BMI to predict their medical charges.

## Data analysis
![image](https://github.com/user-attachments/assets/d382a289-ccae-4353-b5c5-42085f8f02d7)

> It is evident that smoking is a overly influencial feature and population of those who smoke is comparatively lower than those who are nonsmokers. Therefore, smokers and nonsmoker should be considered separately because the small number of outliers of smoker customers would disrupt the causations of the model. 

## Methods
> Linear Regression: A simple model that assumes a linear relationship between the input features (age and BMI) and the target variable (medical charges).
> SGD Regressor: An iterative method for optimizing the linear regression model, which can handle large datasets efficiently.
>
## Conclusion
Both models were trained and evaluated on the dataset. The Linear Regression model had an RMSE of approximately 4662.31, while the SGD Regressor had an RMSE of approximately 4700.45. Although both models performed similarly, the Linear Regression model had a slightly lower RMSE, indicating it provided more accurate predictions for this dataset.

This project demonstrates the process of building and evaluating regression models to predict medical charges, providing valuable insights for determining insurance premiums. Future work could involve exploring more complex models or additional features to further improve prediction accuracy.
