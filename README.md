# eda-statistics
#In this repository I am getting raw data from https://archive.ics.uci.edu/ml/machine-learning-databases/adult/ .
I cleaned this data using the pandas library in python. You can also see the attached eda2.ipynb file in the repository for step by step approach.
First thing I noticed was the raw data was missing its header, therefore, to understand the data more clearly I searched the above mentioned website. From description of the dataset I was able to find appropriate column headings.
After that I tried to find duplicates in the dataset but because of no unique identification of the rows deleting any data was not a good approach.
To interpret data inside the 'Annual_salary' column I converted 'K' into '000' and if it was less than or equal to 50000 then I kept it to 50000 only. If the salary was more than 50000 then I rounded it into 55000. This was done to get a rough idea of the average salary because no more data was provided.
I changed the 'Annual_salary' data column to int from object datatype.
Later I checked any null values in the dataset and found '?' string. To compensate this I added 'NaN' value instead in every column.
I saved the cleaned data into 'Clean_adult_data' file which you can refer to in this repository.
In the last part I analysed the cleaned data regarding the percentage division of every column in different groups. Moreover, I used seaborn library to plot graphs using this data for a clear understanding and outcomes.
