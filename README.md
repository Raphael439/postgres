
# Data Modeling with Postgres
## Purpose and Goals
Sparkify, a startup, is interested in analyzing the data they've been collecting on songs and user activity on their new music streaming app. To do this, they need an easy way to query their data which is currently stored in two local directories of JSON logs and metadata - one on user activity and one on the songs in their app. As a data engineer, you have been asked to create a Postgres database with tables designed to optimize queries on song play analysis, and an ETL pipeline using Python to transfer data from the two directories into these tables. Your role is to define a star schema for the given analytic focus, and write an ETL pipeline that will test your database and ETL pipeline by running queries given by the analytics team and compare your results with their expected results. The first dataset is a subset of real data from the Million Song Dataset which is in JSON format and contains metadata about a song and the artist of that song, and the second dataset consists of log files in JSON format generated by an event simulator based on the songs in the dataset.



 
## How to run the Python scripts
Create tables: run create_tables.py  
Build ETL Pipeline: run etl.py, 
Run test.ipynb to confirm your records were successfully inserted into each table.

## An explanation of the files in the repository
The repository includes the following files:
test.ipynb displays the first few rows of each table to let you check your database.
create_tables.py drops and creates your tables. You run this file to reset your tables before each time you run your ETL scripts.
etl.ipynb reads and processes a single file from song_data and log_data and loads the data into your tables. This notebook contains detailed instructions on the ETL process for each of the tables.
etl.py reads and processes files from song_data and log_data and loads them into your tables. You can fill this out based on your work in the ETL notebook.
sql_queries.py contains all your sql queries, and is imported into the last three files above.
README.md provides discussion on your project.


## schema design 
![image](https://github.com/Raphael439/postgres/blob/main/schema.png)


