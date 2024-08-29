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
## Storage
* HDD / SSD / RAM
* Networking
* Serialization -> turning data into byte streams
```
                                               |-> File
Data -> Serializer --------byte stream---------|-> Data Store
                                               |-> Memory  
```

### Misc
* Distributed computing and storage paradigm
  * MapReduce - Hadoop [Google Research](https://static.googleusercontent.com/media/research.google.com/en//archive/mapreduce-osdi04.pdf)
  * 
