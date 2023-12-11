# Web-Server-Log-Analysis-with-PySpark
This example demonstrates parsing (including incorrectly formated strings) and analysis of web server log data . 

I found many logs at [https://www.sec.gov/dera/data/edgar-log-file-data-set.html](https://www.sec.gov/dera/data/edgar-log-file-data-set.html)
Here I take the 2003 data, because the file is relatively small, about 3-4M. In 2017 the file size is about 300-400M.

Now the project has a new focus. This Jupyter Notebok and production scripts for batch processing serve as investigation steps. The main goal is stream processing of logs with Spark Streams and scheduling with Apache Airflow. 

### Why RDD und Spark Streams?
For historical reasons I decided to keep the project focused on RDDs and Spark Streams. They are suitable for unstructured data. The processing described here will bring the structure to data.

For initially structured data the better tools are DataFrames and StructuredStreams. For those I will find a new playground.

