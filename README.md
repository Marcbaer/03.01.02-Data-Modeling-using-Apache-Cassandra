## Data Modeling with Apache Cassandra

This Project uses an Apache Cassandra database and a python driver to model the streaming data of a music app. The streaming information is provided by csv files.
The architecture of the NoSQL database is optimized for fast reads and the tables are modelled according to three analytical queries:

1. Artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4

2. Name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182

3. User name (first and last) in the music app history who listened to the song 'All Hands Against His Own'


## ETL Pipeline and Data Modeling:

The ETL Pipeline and the Data Modeling are written in the jupyter notebook **[Project_1B_Project_Template.ipynb](Project_1B_Project_Template.ipynb)**.
The notebook copies the provided csv data into a single file **[event_datafile_new.csv](event_datafile_new.csv)**. The CSV is then used to populate the denormalized NoSQL tables streaming_library_01-03.
The design of each individual table is optimized to its corresponding query.
