# WebCaptureDataAnalysis
A simple analysis and visualisation of a log file containing request and network information  1. Used Python to cleanse the data and perform extraction of required information 2. Used Pandas,Numpy,Regex library to perform the above mentioned tasks  # Preprocessing Steps  step 1:importing the raw data file step 2: Creating a dataframe using raw data with one column heading 'Values' step 3:According to the question Only Host,Date,Status code,Bytes is required step 4: Using regular expression "(^\S+)\s" to search for hostname  step 5: Using regular expression "(\d{2}[\/]\w*[\/]\d{4}:\d{2}:\d{2}:\d{2})" to search for date step 6: Using regular expression "\s(\d{3})\s" to search for status code step 7: Using regular expression "\s(\d+)$" to search for bytes step 8: Creating columns called Host, Date,Status,Bytes in Dataframe step 9: Creating new dataframe with only required columns step 10: Printing the No of rows and columns of the dataset step 11: Checking if any of the columns have null values using df.isnull().any() step 12: Only Bytes column has null values  step 13: Finding the number of null values in dataset by summing the nullvalues count step 14: Filling the null values by using df['columnName'].fillna(value,inplace=True) step 15: Formatting the date as required format YYYY/MM/DD HH:MM:SS step 16: Writing the dataframe into csv by using df.to_csv(filepath) and this file is used in tableau to get more insights on the data. step 17: End of preprocessing.
