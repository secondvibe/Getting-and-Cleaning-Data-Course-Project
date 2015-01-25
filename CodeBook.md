# Introduction

`run_analysis.R` performs the following requirements:.

* Merges the training and the test sets to create one data set.
* Extracts only the measurements on the mean and standard deviation for each measurement. 
* Uses descriptive activity names to name the activities in the data set
* Appropriately labels the data set with descriptive variable names. 
* From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

# Variables

* `x_train`, `y_train`, `x_test`, `y_test`, `subject_train` and `subject_test` is the original data from the source.
* `x_data`, `y_data` and `subject_data` is the result of the merged data for analysis.
* `features` contains the appropriate names for `x_data`, which is applied to the column names stored in `mean_and_std_features`, a numeric vector used to extract the desired data.
* Activity names is similar to features and managed through the `activities` variable.
* `x_data`, `y_data` and `subject_data` is merged into all_data for analysis.
* `averages_data` contains the relevant averages which will is exported into a text file.