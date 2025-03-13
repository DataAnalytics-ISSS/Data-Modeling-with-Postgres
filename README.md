Project Overview
-------------------------
Sparkify, a music streaming startup, seeks a SQL analytics database to analyze user listening patterns. Their data, stored as JSON logs (user activity) and metadata (song information), needs to be easily queryable to support insights into user song preferences.

Data Modeling
-------------------------
The database uses a Star Schema with a central fact table, songplays, referencing four dimension tables:
 - Songs
 - Artists
 - Users
 - Time
A relational database is ideal due to the structured JSON format, manageable data size, and the need for SQL-based aggregation and JOIN operations.

Project Structure
-------------------------
The project includes the following key files:

1. create_tables.py: Resets tables by dropping and recreating them.
2. etl.ipynb: Processes a single file to load data into tables; serves as a detailed ETL guide.
3. etl.py: Processes and loads all files based on work in etl.ipynb.
4. README.md: Provides project documentation.
5. sql_queries.py: Contains SQL queries used across scripts.
6. test.ipynb: Verifies table creation and data loading.

Execution Steps
-------------------------
1. Run create_tables.py to set up the database and tables.
2. Run etl.py to process, extract, and insert data.
3. Use test.ipynb to verify data and table structure.