# WebCaptureDataAnalysis

A simple analysis and visualisation of a log file containing request and network information
<br>

1. Used Python to cleanse the data and perform extraction of required information <br>
2. Used Pandas,Numpy,Regex library to perform the above mentioned tasks <br>


# Preprocessing Steps
<br>

step 1:importing the raw data file <br>
step 2: Creating a dataframe using raw data with one column heading 'Values' <br>
step 3:According to the question Only Host,Date,Status code,Bytes is required <br>
step 4: Using regular expression "(^\S+)\s" to search for hostname <br>
step 5: Using regular expression "(\d{2}[\/]\w*[\/]\d{4}:\d{2}:\d{2}:\d{2})" to search for date <br>
step 6: Using regular expression "\s(\d{3})\s" to search for status code <br>
step 7: Using regular expression "\s(\d+)$" to search for bytes <br>
step 8: Creating columns called Host, Date,Status,Bytes in Dataframe <br>
step 9: Creating new dataframe with only required columns <br>
step 10: Printing the No of rows and columns of the dataset <br>
step 11: Checking if any of the columns have null values using df.isnull().any() <br>
step 12: Only Bytes column has null values <br>
step 13: Finding the number of null values in dataset by summing the nullvalues count <br>
step 14: Filling the null values by using df['columnName'].fillna(value,inplace=True) <br>
step 15: Formatting the date as required format YYYY/MM/DD HH:MM:SS <br>
step 16: Writing the dataframe into csv by using df.to_csv(filepath) and this file is used in tableau to get more insights on the data. <br>
step 17: End of preprocessing. <br>


![Visualisation 1](https://github.com/swathiravi10695/WebCaptureDataAnalysis/blob/main/VisualPlot1.png)
<br>

![Visualisation 2](https://github.com/swathiravi10695/WebCaptureDataAnalysis/blob/main/VisualPlot2.png)

