# Data Engineering Nanodegree Project 2: Data Modeling with Cassandra

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. 

Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

This project aims on creating an Apache Cassandra Database where we can create queries to answer the questions.


## Getting Started

Pre-requisites:

- Python 3
- [Cassandra running locally](https://cassandra.apache.org/doc/latest/cassandra/getting_started/installing.html)
- [Cassandra python client](https://github.com/datastax/python-driver)

## Dataset

For this project, you'll be working with one dataset: event_data. The directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:

```
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
```

Here is the example of one row of data:

```
Deepest Blue,Logged In,Tegan,F,16,Levine,210.54649,paid,"Portland-South Portland, ME",PUT,NextSong,1.54079E+12,481,Deepest Blue,200,1.54206E+12,80
```

## Project Repository Files
### main.ipynb
Jupyter notebook that models a Cassandra Database, perform a ETL proccess and execute queries to answer 3 questions:
1. Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4
2. Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

