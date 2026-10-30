# My-first-SQL-querry
# Overview
- In this scenario, you have to determine which employee devices must be updated. You also need to investigate user login activity to explore if any unusual activity has occurred.
# Data
- The information you need is located in the machines and login_attempts tables in the organization database.
# Task 1. Retrieve employee device data: In this task, you need to obtain information on employee devices because your team needs to update them. The information you need is in the machines table in the organization database.
SELECT *
FROM machines;

# Run the following query to select only the device_id and email_client columns from the machines table.
SELECT device_is, email_client
FROM machines;

# Complete the query to return only the device_id, operating_system, and OS_patch_date columns from the machines table.
SELECT device_id,operating_system,OS_patch_date
FROM machines;

# Task 2: Investigate login activity
- Write a SQL query to select the event_id and country columns from the log_in_attempts table.
SELECT event_id, country
FROM log_in_attempts

# check if login attempts were made outside of the organization's working hours.
- Write a SQL query that selects the username, login_date, and login_time columns from the log_in_attempts table.
SELECT username, login_date, login_time
FROM log_in_attempts;

- Write a SQL query that selects all columns from the log_in_attempts table, using a single symbol after the SELECT keyword.
SELECT *
FROM log_in_attempts

# Task 3. Order login attempts data - sort the information by date
- Run the following query, which orders log_in_attempts data by login_date:
SELECT *
FROM log_in_attempts
ORDER BY login_date

- Modify the query from the previous step by adding the login time to the ORDER BY clause. You must replace X with the appropriate column name:
SELECT *
FROM log_in_attempts
ORDER BY login_date, login_time;



