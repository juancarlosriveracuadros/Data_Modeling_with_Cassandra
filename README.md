# Data_Modelling_with_Cassandra
Data Modelling for the company Sparkify. The data is a collection of songs and user activities on their new music streaming app. The goal of the program is to understand what songs users are listening to.The information comes from a directory of CSV files. The program is to created a data base in Apache Cassandra. The pipeline was writed in Python and the program is in a Jupyter Notebook (Data_Modeling_with_Cassandra.ipynb).

## Datasets 
dataset: event_data. The directory of CSV files partitioned by date.

### Steps in (Project_1B_ Project_Template.ipynb)
1) all the data is grouped in event_datafile_new.csv 
    The columns are: artist, firstName, gender, itemInSession, lastName, length, level, location, sessionId, song, userId 
2) The program create a new keyspace (udacity) for creation of the work tables
3) Creat the queres and the tables to answer the three questions
4) test the tables and queries

### Questions 
Query 1:  Give me the artist, song title and song's length in the music app history that was heard during \
          sessionId = 338, and itemInSession = 4
          query 1 name: sessionId_338_4

Query 2: Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name)\
         for userid = 10, sessionid = 182
         query 2 name: userid_10_sessionid_182

Query 3: Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'
         query 3 name: listening_all_hands_against_his_own
