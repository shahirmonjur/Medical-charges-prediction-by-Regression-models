## Problem Statement

> ACME Insurance Inc. offers affordable health insurance to thousands of customer all over the United States. 

> This is primarily a data analysis and feature analysis notebook that also trains regression models to predict the medical charges of a customer of the insurance company given their data like age, BMI, how many children they have.
>
> Estimates from this system will be used to determine the annual insurance premium (amount paid every month) offered to the customer. Due to regulatory requirements, the insurance company must be able to explain why their system outputs a certain prediction.
>
> We have found a [CSV file](https://raw.githubusercontent.com/JovianML/opendatasets/master/data/medical-charges.csv) containing verified historical data, consisting of the aforementioned information and the actual medical charges incurred by over 1300 customers.

> Dataset source: https://github.com/stedy/Machine-Learning-with-R-datasets

## Dataset Description
> The dataset contains information about 1,338 customers, including their age, sex, BMI, number of children, smoking habits, region of residence, and annual medical charges. For this project, we focus on non-smokers and use their age and BMI to predict their medical charges.
<img src="https://i.imgur.com/87Uw0aG.png" wi![newplot(2)](https://github.com/user-attachments/assets/e967b4e7-4e59-4157-b1d6-49ed2712b82d)
dth="480">
## Data analysis
![image](https://github.com/user-attachments/assets/d382a289-ccae-4353-b5c5-42085f8f02d7)

> It is evident that smoking is a overly influencial feature. Therefore, smokers and nonsmoker should be considered separately because the small number of outliers of smoker customers would disrupt the causations of the model. 
![newplot(3)](https://github.com/user-attachments/assets/d24519a4-b258-4346-89f1-83013027e8c3)

## Methods
> Linear Regression: A simple model that assumes a linear relationship between the input features (age and BMI) and the target variable (medical charges).
> SGD Regressor: An iterative method for optimizing the linear regression model, which can handle large datasets efficiently.
>
## Conclusion
>Both models Linear regression and SGD Regressor were trained and evaluated on the dataset. The Linear Regression model had an RMSE of approximately 4608.57, while the SGD Regressor had an RMSE of approximately 4608.61. Both models performed similarly, probably because we worked with few features.

![image](https://github.com/user-attachments/assets/a2c7aaa6-516d-4e52-9985-e2dfbba1b30b)

>This project demonstrates the process of building and evaluating regression models to predict medical charges, providing valuable insights for determining insurance premiums. 
