# Project 1: Data Modeling with Postgres

## How to run

- Install python3, postgresql, psycopg2, ,pandas
- Run:

```python
python3 create_tables.sql
python3 etl.py
```

## Overview

We create a database that help music streaming startup called Sparkify to handles music data. Data is a set of JSON files.

After create database, we builds an ETL pipeline to extract data from JSON files, transform and load into database.

## About database

### Fact Table

- **songplays**: song play data together with user, artist, and song info (songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent)

### Dimension Tables

- **users**: user info (columns: user_id, first_name, last_name, gender, level)
- **songs**: song info (columns: song_id, title, artist_id, year, duration)
- **artists**: artist info (columns: artist_id, name, location, latitude, longitude)
- **time**: detailed time info about song plays (columns: start_time, hour, day, week, month, year, weekday)
