## Data Modeling with Postgres

### Introduction

Sparkify want to analyze their data they've been collectiong on songs and user activity on their music streaming app. They are particularly interested in understanding what songs userss listen to. User activity is stored in a directory of JSON logs and their is JSON metadata about the songs on the app. However they have no easy way to query the data. In this project data is modelled in a Postgres database and an ETL pipeline is created. 


### Schema

The schema is as below for the Sparkify database, it utilises a star schema with song_plays as a fact table and users, artists, time and songs all dimension tables

![Blank diagram (1)](https://user-images.githubusercontent.com/46905748/103463089-bcb26700-4d21-11eb-9be5-2f56bd982a11.png)

### How to run

The assumption is made you already have a Postgres database up and running. 

1. Run create_tables.py to prepare the database.
2. Run etl.py to insert values into database.
3. Run test.ipynb to check if the above has worked.

n.b. the etl.ipynb was used for development.
