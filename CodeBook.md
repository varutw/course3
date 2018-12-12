CodeBook


This file explains how run_analysis.R works, as following: 

1. It reads X data that is collected from the accelerometers from the 30 Samsung Galaxy S smartphone

users, in different activities. The X data has numerous kind of features. run_analysis.R reads both 

test set and train set, and then merge into one dataset.
 
2. Then it selects only the features that are related to mean and standard deviation and create new dataset,

but excludes meanFreq, which its purpose is not about the mean by its definition.

3. After that, run_analysis.R calculates the average value of each selected features, for each

subject and activity. 

4. Finally, it creates tidyDataSet text file as an outcome.






