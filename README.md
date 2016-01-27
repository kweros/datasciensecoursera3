# datasciensecoursera3
Getting and Cleaning Data Course Project

This file describes how run_analysis.R script works.

1- Download file from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and unzip data.

2- Rename the folder with "data". Make sure the folder "data" and the run_analysis.R script are both in the current working directory.

3- Use source("run_analysis.R") command in RStudio. That will generate two output files in the current working directory: 
   - merged_data.txt (7.9 Mb), that contains a data frame called cleanedData;
   - data_with_means.txt (220 Kb): it contains a data frame called result.

4- Use data <- read.table("data_with_means.txt") command in RStudio to read the file. Since we are required to get the average of each variable for each activity and each subject, and there are 6 activities in total and 30 subjects in total, we have 180 rows with all combinations for each of the 66 features.
