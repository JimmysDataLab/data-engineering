# data-engineering
Everything about modern data engineering
```
                                                            -> Analytics
Generation ->  Ingestion -> Transformation -> Serving       -> ML/AI
               -----------------------------------------    -> Reverse ETL
                               Storage
```
## Data generation (source systems)
* structured / unstructured data
* Relational database / Non-relational database / Key-value store
* Third-party systems and event streams
  * event streaming
  * Idempotency
  * AWS SQS, Kinesis, RabbitMQ, Kafka, Spark
# Storage
* HDD / SSD / RAM
* Networking
* Serialization -> turning data into byte streams
  * Row based serialization / column based serialization
* Types of storage -> File, block, object, cache, stream
 ```
                                               |-> File
Data -> Serializer --------byte stream---------|-> Data Store
                                               |-> Memory  
```
* Distributed storage + Distributed compute
  * S3, Spark, Redshift, snowflake
* Row based vs columnar storate (OLTP vs OLAP)
### Data warehouse, lake, lakehouse
* Data Warehouse
  *  Mostly used of structured data, business analytics
  *  OLAP
  *  preprocessed
  *  eg: redshift, BigQuery, snoflake
* Data Lake
  * Unstructured and structured
  * Store it first ,look later
  * eg : s3
* Data lakehouse
  * best of both worlds
  * eg : s3 + ICEBERG, DELTA LAKE
  * Nowadays we can see separation between storage and compute Eg: Trino

* Data storage lifecycle - hot, warm, cold
# Ingestion
* Moving data from source system to storage systems.
* Batch / Micro-batch / Streaming
* ETL / ELT
## Ways to injest data
* DB connection JDBC
* CDC Postgresql Mysql
* 



### Misc
* Distributed computing and storage paradigm
  * MapReduce - Hadoop [Google Research](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf)
  * 
