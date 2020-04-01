# Data Modeling with Cassandra



## **Overview**
For this project, Data Modeling with Cassandra and complete an ETL pipeline using Python. To complete the project, I'm need to model o data by creating tables in Apache Cassandra to run queries.


## **Datasets**

**event_data**
Sample Record :
```
{"artist": "", "auth": "Logged In", "firstName": "Walter", "gender": "M", "itemInSession": 0, "lastName": "Frye", "length": "", "level": "free", "location": "San Francisco-Oakland-Hayward, CA", "method": "GET", "page": "Home", "registration": 1.54092E+12, "sessionId": 38, "registration": "", "sessionId": "200", "song": "", "status": "", "ts": , "userId": ""}
```



## **Schema Tables**

**song_by_session**  - songs session of table
```
session_id, item_in_session, artist_name, song_title, song_duration
```

**user_song_by_id**  - user and song of table
```
user_id, session_id, item_in_session, artist_name, song_title, user_first_name, user_last_name
```

**user_listing_song**  - user lisnting song of table
```
user_id, user_first_name, user_last_name, song_title
```



## Project Files

```etl.ipynb``` -> Jupyter notebook read and process files **event_data** and output create file **event_datafile_new.csv** to run ETL and process queries for answers to questions. 

```event_datafile_new.csv``` -> Create file output for get data to tables



## How to run

Run the files ```etl.ipynb```, open jupyter notebook and running all cells.
