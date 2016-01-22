# GCD_CP
Getting and Cleaning Data - Course Project

This README.md file explains how run_analysis.R works.

1. Unzip the data from:
      ttps://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and rename the folder with "data".
      Make sure the folder is in the current working directory.
2. Source("run_analysis.R") in RStudio.
3. Two output files will be generated in the WD:
      * merged_data.txt : it's a data frame called cleanedData with 10299*68 dimension.
      * data_with_means.txt : it's a data frame called result with 180*68 dimension.
4. Use data <- read.table("data_with_means.txt") command in RStudio to read the file.

Since we are required to get the average of each variable for each activity and each subject:
* There are 6 activities in total and 30 subjects in total, we have 180 rows with all combinations for each of the 66 features.
