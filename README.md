#Getting and Cleaning Data

##Coursera Course: Getting and Cleaning Data

Assignment Submission Files

* README.md
* CookBook.md
* run_analysis.R
* tidy.txt


The data in the "Human Activity Recognition Using Smartphones Dataset Version 1.0" have been taken from experiments carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz data were captured. The experiments were video-recorded to label the data manually. The obtained dataset was randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

See also http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

##List of the operations done to achieve the outputs:

* Downloaded the data set
* Unzipped the data set into my chosen working directory
* Loaded test and training data sets into data frames
* Loaded source variable names for test and training data sets
* Loaded activity labels
* Combined test and training data frames using rbind
* Paired down the data frames to only include the mean and standard deviation variables
* Replaced activity IDs with the activity labels for readability
* Combined the data frames to produce one data frame containing the subjects, measurements and activities
* Produced "merged_tidy_data.txt" with the combined data frame as the first expected output
* Created another data set using the data.table library to easily group the tidy data by subject and activity
* Then applied the mean and standard deviation calculations across the groups
* Produced "calculated_tidy_data.txt" as the second expected output
* Please refer to run_analysis.R for implementation details.
