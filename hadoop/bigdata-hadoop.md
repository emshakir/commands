## Import data from mysql to HDFS Using sqoop

sqoop import --connect jdbc:mysql://localhost/databasename --driver com.mysql.jdbc.Driver 
--table <table_name> -m 1 
--username xxx --password xxxxx

NOTE: -m 1 => Number of Mapper, not required on real cluster

## Import data from mysql to HIVE Using sqoop

sqoop import --connect jdbc:mysql://localhost/databasename --driver com.mysql.jdbc.Driver 
--table <table_name> -m 1 
--username xxx --password xxxxx 
--hive-import

## Export Data from Hadoop to mySQl using sqoop

sqoop export --connect jdbc:mysql://localhost/databasename --driver com.mysql.jdbc.Driver -m 1 
--table <table_name > --export-dir <directory> 
--input-fields-termibated-by '\001'<delimeter> 
--username xxx --password xxxxx


## Big Data Tools

- Impala(Alt to Hive)
- Accumulo(Alt to Hbase)
- Redis(Caching)
- Ignite(Alt to redis, allows ACID, SQL support done in memory)
- Elastic search(Distriibuted document search and analytics engine)
- Kinesis(AWS version of kafka)
- Apache NiFi
- Falcon(Organize the floe of data within Hadoop(used with oozie))
- Apache Slider(Deployment tool for yarn cluster)
