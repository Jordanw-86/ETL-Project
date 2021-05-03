# ETL-Project Movie Madness


## Project Proposal
We going to look a 3 databases, 2 from IMBD and 1 from a rotten tomatoes ratings database. We will drop any unneeded columns, and load these 3 tables into SQL and join them on Movie ID /Director/Actor.

## Extractions
For the clean up process we imported the raw CSVs into pandas and dropped any unneeded columns from all the databases. From there, we created a schema using Postgres and imported the tables into SQL where we joined these databases on movie id/actor/director.

## Transform
 For this project I removed a duplicate columns in the process of cleaniong the 3 CSV files. Once I got the dataframes clean, I  remained columns merge on movie title. This allows me to join on this columns in Postgres.



## Load
For loading this data, I used a bit of SQLalchamy "df_rt.to_sql(name='rotten_tomatoes', con=engine, if_exists='append', index=False) in order load these new dataframes into SQL

