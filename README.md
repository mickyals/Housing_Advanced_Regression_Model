# Suprise Housing Australian Market Regression Model
> A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia

## Business Goal
> To model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

> The company wants to know:
 - Which variables are significant in predicting the price of a house, and
 - How well those variables describe the price of a house.


## Table of Contents
| File name | Description | Format |
|-----------|-------------|--------|
|definition | data dictionary for fields in dataset| txt|
|train| training dataset | csv|
|  House_Price_Prediciton_Mickell_Als   |      notebook            |   ipynb |
| Subjective Questions | repsonses to questions | pdf|


## Conclusion

#### Ridge Model Statistics
- alpha = 0.7
- r-squared train:  0.9157301643105313
- r-squared test:  0.8927063601032452
- number of significant features in Ridge: 50 out of 180 total features


#### Lasso Model Statistics
- alpha = 0.0001
- r-squared train:  0.9142013811213581
- r-squared test:  0.8977191255593224
- number of significant features in Lasso: 36 out of 180 total features

#### Top 5 Significant Features by Model

| Ridge Regression | Lasso Regression |
|------------------|------------------|
|GrLivArea         |GrLivArea         |
|TotalBsmtSF       |OverallQual-9     |
|OverallQual-9     |OverallQual-10    |
|HomeAge           |TotalBsmtSF       |
|BsmtFullBath-2    |HomeAge           |