clean_getting_course
====================
The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set.

The data was collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

The script is called run_analysis.R. It generates the first tidy set that was requested for the assignment: merge both the training and test sets with only the measurements on the mean and standard deviation for each variable.

The algorithm is:
a) Read the training set of measurements into a data frame called "X_train".
b) Use the feature set names in file "features.txt" to rename each of the 561 variables.
c) Create a new data frame called "trainMainset" extracting only the columns whose names contain the word "mean" or "std".
d) Read the subject associated with each row of the training set into a data frame "subject_train" and rename the column as "Subject".
e) Read the activity associated with each row of the training set into a data frame "y_train" and rename the column as "Activity". 
f) Merge the above data frames "X_train", "subject_train" and "y_train" as one data frame called trainingSet using function cbind.
g) Repeat the above steps for the test set using the corresponding files "X_test.txt", "subject_test.txt" and "y_test.txt".
h) Merge the rows of the training and test set into a single data frame of 10299 rows (+header) and 81 variables.
i) Write the results in a file called "mean_std_measurements_tidydata.txt".

Unfortunately, I was not able to complete the second part of the assignment: create a second, independent tidy data set with the average of each variable for each activity and each subject. 


