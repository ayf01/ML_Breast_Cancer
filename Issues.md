## Issues:
##### Data is imbalanced.
- undersampling is not possible since data is not large
- oversampling by duplicating data is possible, but may lead to overfitting
- use metrics like f1-score

##### Feature Selection:
- skip in neural network models
- is different than Dimensionality reduction
    
##### Null values in data
- drop rows that contain null values -> data loss
- check feature by feature, if it contains a lot of null values (60-70%), drop the feature/column
- SimpleImputer (or any imputer) to replace NaNs with most frequent category.
-  depending on data, one can create a custom function to replace NaNs with nearest X Most frequent Non-NaN category
- if the feature that is null is numerical: Plot the histogram of the feature and then deduce the result:
    1. If left-skewed then use median as replacement
    2. If right-skewed then use median as replacement
    3. If normal distribution, then can use mean/median
- we impute null value on the whole data not only training.. we should impute after reducing dimensionality


##### nominal data -> hot encoding, ordinal data -> label encoding
- Label Encoding might represent them as:
Red -> 0
Yellow -> 1
Blue -> 2
- One-Hot Encoding would create separate columns for each category:
Color_Red with values [1, 0, 0]
Color_Yellow with values [0, 1, 0]
Color_Blue with values [0, 0, 1]
->>> dimensionality problem
        
##### Even with tuning hyperparameters, we did not reach satisfying results.
- finetune an existing pre-trained model 

##### When should we encode data? before or after splitting? what if in test data a new category was introduced?