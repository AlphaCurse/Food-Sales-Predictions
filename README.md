# Food Sales Predictions
## Predict Outlet Sales with Dataset

**Author**: Tyler Brown

### Business Problem:
Retailer would like to predict sales utilizing the properties of products and outlets provided in the dataset.

### Data:
File sales_predictions.csv within the repository contains data used for determining sales predictions.
To help the retailer, our goal is to predict the "Item_Outlet_Sales" column. The remaining columns will be used to determine the prediction.

## Methods:
-"Item_Identifier" column was dropped from the dataset due to unique categorical values, which would cause errors in making predictions.

-Fill missing values in column "Item_Weight" with the median numerical value. The percentage of data loss is high and would have a big impact on the results.

-Fill missing values in column "Outlet_Size" with the median categorical value "Medium". The percentage of data loss is high and would have a big impact on the results.

-Column "Item_Fat_Content" contains inconsistent categories, where "LF" and "low fat" can translate to "Low Fat". Similarly, "reg" can translate to "Regular".

## Results:
#### Amount Per Item Type
![Item_Type_Image](ItemTypeAmount.png)

All item types presented in the data are displayed to visualize the difference in the amount of each item type.

#### Item Visibility Amount per Item Fat Content
![Vis_Per_Fat_Image](ItemVisPerFatContent.png)

The graph displays the Item Fat Content when compared with its visibility from the dataset.

#### Item Visibility Correlation within Dataset
![Correlation_Image](Correlation.png)

From the correlation graph, we can determine little correlation between most of the columns in the dataset. The best correlation between two different columns of data would be "Item_Outlet_Sales", which is our goal for predictions, and "Item_MRP".

## Recommendations:
I recommend implementing the Regression Tree model for this specific dataset. 
As we are aware, categorical variables exist within our dataset. Being the case, Linear Regression models cannot take categorical variables as easily when compared to the Regression Tree model. 
The Regression Tree is easier to interpret and will work with missing data unlike Linear Regression models, which would ignore the missing values. 

## Limitations & Next Steps:
- Presented with missing values in the dataset
- No additional data is available for greater accuracy in predictions

The next steps would be to inform the retailer on the results of predictions based on the dataset. If satisfied, the retailer can use these predictions and determine future value in sales for the business.
If displeased, the retailer can make necessary arrangements to produce greater value in sales.

### For further information...
If there are any additional questions, I can be contacted at alpha.curse@gmail.com
