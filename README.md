Databricks_Data_Engg
Basic Data Engineering steps taken in this project:
1.Importing important libraries
2.importing datasets
3.checking for nulls in the columns 
4.filtered all null values to deal with it
5.filtered a row with null description where stockcode is 22139 to check that all value in description is null for given stockcode
6.distinct stock code and description to find out how many values can be filled 
7.window function to partition data based on description
8.filled the Nan values with with the last non-null value within the same stockcode
9.check that it worked or not in my case nan value was 166 and after using the operation to fill nan it dropped to 47
10.After that repeated step 5 to recheck
11.created another dataframe from same dataframe to perform other operations
12.created a new column TotalPrice to find the amount of stock buyed by a single customer
13.Renamed column description to desc and sum the quantity of stock using GroupBy on Description and orderBy Quantity asc =false
