# Suprise Housing Australian Market Regression Model
> A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia

## Business Goal
> To model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## Table of Contents
| File name | Description | Format |
|-----------|-------------|--------|
|definition | data dictionary for fields in dataset| txt|
|train| training dataset | csv|
|  House_Price_Prediciton_Mickell_Als   |      notebook            |   ipynb |
| Subjective Questions | repsonses to questions | pdf|


## Conclusion

#### Ridge Model
- alpha = 2.0
- r-squared (train) = 0.9414316518539076
- r-squared (test) = 0.9052748083288656
- number of significant features in Ridge: 147 out of 234 total features (based on abs_value > 0.01)


#### Lasso Model
- alpha = 0.0001
- r-squared (train) = 0.9403512453236479
- r-squared (test) = 0.9067890182321706
- number of significant features in Lasso: 136 out of 234 total features

#### Top 5 Features by Model

| Ridge Regression | Lasso Regression |
|------------------|------------------|
|GrLivArea         |GrLivArea         |
|TotalBsmtSF       |OverallQual-9     |
|OverallQual-9     |OverallQual-10    |
|HomeAge           |TotalBsmtSF       |
|BsmtFullBath-2    |HomeAge           |