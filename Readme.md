This is the capstone assignment for the Getting and Cleaning Data Coursera Course

Files

    Readme.md is this file being read right now. It is a general outline of the project, and it's contents and solutions.

    CodeBook.md a code book that describes the variables, the data, and any transformations or work that I performed to clean up the data

    run_analysis.R prepares the data and the 5 steps required as outlined in the assignment

    tidy_data.txt is the exported final data after going through all the sequences in the script and codebook.

run.analysis.R Tutorial

    Step 1:
        Reads and then merges the training and test sets to create one data set

    Step 2:
        Extracts just the mean and standard deviations for each measurement on the merged data

    Step 3:
        Read the activity labels from activity_labels.txt and replace the numbers with the text. Uses gsub function to replace activity abbreviations with mnemonic descriptions
        

    Step 5:
        Create a new data frame by finding the mean for each combination of subject and label. It's done with group_by and summarize functions

    Final step:
        Write the new tidy set into a text file called tidy_data.txt

