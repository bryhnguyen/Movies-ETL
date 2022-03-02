# Movies-ETL

# Overview

This project practices the Extact-Transform-Load process using Python and Pandas to extract data from .csv files and a Wikipedia .json file into a dataframe that can be transformed and cleaned up to present in a more accurate, consistent, and presentable way to be stored into a postgreSQL database. The process began by writing functions to convert the metadata .csv files into a dataframe and another function to convert the wikipedia .json file into raw data before it could be converted into a dataframe as well. Then, once we have the data converted to dataframes to be manipulated, regular expressions were used to clean the data to identify discrepancies with formatting, currencies, and drop any values that were not relevant to the movies database to be created and loaded into. After the dataframes were cleaned, they can then be merged into one dataframe to undergo final cleaning and filling of any null values with a '0'. Finally, the merged and cleaned dataframe can be merged into the postgreSQL database by establishing a connection.

# Results

We can confirm that the PostgreSQL database was created and loaded successfully by using the select count * query from the movies and ratings tables.  

![alt text](https://github.com/bryhnguyen/Movies-ETL/blob/main/Resources/movies_query.png)

![alt text](https://github.com/bryhnguyen/Movies-ETL/blob/main/Resources/ratings_query.png)
