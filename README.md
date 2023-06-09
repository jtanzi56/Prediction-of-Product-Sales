# **Grocery Sales Prediction**
## Build a predictive model and predict the sales of each product at a particular outlet

- **Author:** Jacob Tanzi 

### Retailer wants to understand the properties of products and outlets which play a key role in sales.:
## **Project Desciption**
### **Overview**
Using the Grocery Data we will, load and clean the data. Explore data analysis, explore visuals, pre process for machine learning, create machine learning pipelines, and test multiple machine learning models.


### **Data Source**
The data was sourced from [analyticsvidhya.com](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/)

There are 8523 rows, and 12 columns.
The rows represent 8523 observations, and the columns represent 11 features and 1 target variable.

### **Data Dictionary**
- **Item_Identifier:** Unique product ID
- **Item_Weight:** Weight of product
- **Item_Fat_Content:** Whether the product is low fat or regular
- **Item_Visibility:** The percentage of total display area of all products in store allocated to the particular product
- **Item_Type:** The category to which the product belongs
- **Item_MRP:** Maximum Retail Price (list price) of the product
- **Outlet_Identifier:** Unique store ID
- **Outlet_Establishment_Year:** The year in which store was established
- **Outlet_Size:** The size of the store in terms of ground area covered
- **Outlet_Location_Type:** The type of area in which the store is located
- **Outlet_Type:** Whether the outlet is a grocery store or some sort of supermarket
- **Item_Outlet_Sales:** Sales of the product in the particular store. This is the target variable to be predicted.


## Methods
- Data was prepared by correcting null values, fixing inconsistencies, and dropping unnecessary columns  
-The data preperation allowed the exploratory analysis to focus on Item_Type, Item_Outlet_Sales, Outlet_Type

## Results

### Exploratory Data Analysis
-While exploring data a heatmap was made of any correlations of numeric data
-Looked at what Outlet Type preformed the best overall
-Did that Outlet Type out preform in all Item Type

#### Heatmap of correlations
<p align = "center"> 
  <img src = "https://github.com/jtanzi56/Prediction-of-Product-Sales/blob/d685b5e055ee6a99c580b5e35ef55d67f55b16f6/heatmap.png">
</p>

>Heatmap used to visualize any correlations between, item weight, item visibility and item outlet sales.


#### Sales by Outlet Type
<p align = "center"> 
  <img src = "https://github.com/jtanzi56/Prediction-of-Product-Sales/blob/157d61cdf7320a30e4bdf66fd52497630dae09ba/sales.by.outlet%20type.png">
</p>
Supermarket 3 'Outlet Type' was preforming the best

#### Item Type Sales by Outlet Type
<p align = "center"> 
  <img src = "https://github.com/jtanzi56/Prediction-of-Product-Sales/blob/157d61cdf7320a30e4bdf66fd52497630dae09ba/item.type.byoutlet.png">
</p>
Supermarket Type 3 out preforms all other Outlet Types in all Item Types, with the exception of Seafood.



### Maching Learning Using the Following Models:
    - Linear Regression Model
    - Lasso Linear Regression Model
    - Decision Tree Regressor Model
    - Decision Tree Tuned Regressor Model
    - Bagged Tree Regressor Model
    - Random Forest Regressor Model
    

## Models Evaluated & Results

Linear Regression Test Scores
MAE: 804.9629 
MSE: 1,196,932.5739 
RMSE: 1,094.0441 
R2: 0.5662

Lasso Linear Test Scores
MAE: 803.7264 
MSE: 1,194,063.4234 
RMSE: 1,092.7321 
R2: 0.5672

Decision Tree Test Scores
MAE: 1,065.2825 
MSE: 2,403,008.5516 
RMSE: 1,550.1640 
R2: 0.1290

Decision Tree Tuned Test Scores
MAE: 738.2100 
MSE: 1,115,558.0387 
RMSE: 1,056.1998 
R2: 0.5957


Bagreg Tree Test Scores
MAE: 814.2355 
MSE: 1,373,290.9707 
RMSE: 1,171.8750 
R2: 0.5022

Random Forest Test Scores
MAE: 795.2895 
MSE: 1,308,147.1894 
RMSE: 1,143.7426 
R2: 0.5259



## Recommendations:
I recommend the Random Forest Model out of the current regression options. While it does have some bias, accounting for just 53% of the variations tested. It out preformed the linear(by far) and the tree model.

I believe we achived the goal to help the retailer understand the properties of products and outlets that play crucial roles in predicting sales.

As seen in these features used by the Random Forest Model

Item_Weight
Item_MRP
Item_Fat_Content_Low Fat
Item_Fat_Content_Regular
Item_Type_Baking Goods
Item_Type_Breads
Item_Type_Breakfast
Item_Type_Canned
Item_Type_Dairy
Item_Type_Frozen Foods
More of your own text here


## Next Steps
Will continue to analyze machine learning models to find best balance of bias and variance. As more data becomes avaliable I am confident the Random Forest Model will continue to improve. 



### For further information


For any additional questions, please contact:
-Jacob Tanzi
**Jtanzi56@gmail.com**
