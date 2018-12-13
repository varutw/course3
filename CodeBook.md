CodeBook


This file explains the input, and output procesure of how run_analysis.R works.


INPUT

the files that are used as input in this project are as following:

	- features.txt
	- activity_labels.txt
	- X_train.txt
	- y_train.txt
	- X_test.txt
	- y_test.txt
	- subject_train.txt
	- subject_test.txt

X data (X_train.txt y_train.txt) is collected from the accelerometers and gyroscope from 

the 30 Samsung Galaxy S smartphone users (subject_train.txt and subject_test.txt), 

in different activities (indicated in activity_labels.txt). The data from accelerometer and gyroscope is

calculated into different features (listed in features.txt)


OUTPUT PROCEDURE


1. run_analysis.R reads both all test and train dataset, and then merge into one dataset called "dataNew".
 
2. Then it selects only the features that are related to mean and standard deviation 

and create new dataset, but excludes meanFreq, which its purpose is not about the mean by its definition.

This new vector is called "featuresNew". It then extract the column of "dataNew" dataframe with "featuresNew"

vector.

3. After that, run_analysis.R calculates the average value of each selected features, for each

subject and activity of "dataNew" dataframe, rename and rearrange in order to obtain new dataset 

called "dataComplete". In this process, it also replace the names of activity that are indicated in 

activity_labels.txt, instead of number.

4. Finally, it creates tidyDataSet text file from dataComplete dataset as an outcome of this project.






