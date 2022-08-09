# Movies-ETL

Extract, transform, load process using Python and SQL

## Overview

The project included extracting a large data set from several online sources, then transforming the data into a usable dataset for a "hacking competition." Once the data was transformed and narrowed in scope for the hackathon, the DataFrames were loaded into PostgreSQL.

## Resources

- Data files: wikipedia-movies.json, movies_metadata.csv, ratings.csv
- Software: Python, Jupyter Notebook, PostgreSQL, pgAdmin

## Deliverable One

Using knowledge of Python, Pandas, the ETL process, and code refactoring, a function was written that reads in the three data files and creates three separate DataFrames. This function was written in Jupyter Notebook in the file ETL_function_test.ipynb.

## Deliverable 2

Using knowledge of Python, Pandas, the ETL process, and code refactoring, the Wikipedia data was extracted and transformed in order to be merged with the Kaggle metadata. In order to properly extract the IMDb IDs, a regular expression string was used, duplicates were dropped, and a try-except block was utilized to catch errors. This function was written in Jupyter Notebook in the file ETL_clean_wiki_movies.ipynb.

## Deliverable 3

Using knowledge of Python, Pandas, the ETL process, and code refactoring, several pandas dataframes were created. After extracting and transforming the Kaggle and MovieLens rating data, first a movies_df dataframe was created consisting of merged Kaggle metadata and Wikipedia movies dataframe. Next a merged rating data dataframe with the movies_df dataframe into a movies_with_ratings_df dataframe was created. This function was written in Jupyter Notebook in the file ETL_clean_kaggle_data.ipynb.

## Deliverable 4

Using knowledge of Python, Pandas, the ETL process, code refactoring, and PostgreSQL, the movies_df DataFrame and MovieLens rating CSV data was added to a SQL database. This function was written in Jupyter Notebook in the file ETL_create_database.ipynb. Confirmation that the tables were properly added to SQL can be seen by the total number of rows for [the movies table](https://github.com/josephrodini/Movies-ETL/blob/main/Resources/movies_query.PNG) and [the ratings table](https://github.com/josephrodini/Movies-ETL/blob/main/Resources/ratings_query.PNG).

## Summary

The extract, transform, load function created collects and cleans movie data from different sources (Wikipedia JSON and Kaggle and ratings CSV files), then transforms and merges the data and loads it into two PostgrSQL tables ready to be used by the hackathon participants for their analysis.

