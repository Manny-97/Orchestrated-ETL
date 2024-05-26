# Orchestrated-ETL

## Problem statement:

The raw structured data is stored in CSV files. We want to pre-process this data, clean the data, and store it in the database. In this case, the database is PostgreSQL. In many situations, the data keeps changing or new data is added to the system. In such cases, our CSV files will also change with a frequency equal to the frequency of new data coming in. We would then need to run the data preprocessing script and then load the data into our destination data store (PostgreSQL).

All the above-mentioned tasks would need to be well orchestrated, scheduled, and then executed. For this, we use an orchestration tool — Apache Airflow. To use all these tools and to perform our tasks, we would need a hosting environment. In this project, we will use Docker as our hosting environment. All the tools will be run as Docker containers. All the code will be written in Python.