# pyspark_cluster
PySpark With Cluster

# Connect Pyspark with Spark Remote
```
from pyspark.sql import SparkSession
spark2 = (SparkSession.builder
    .appName("JupyterSparkExample")
    .remote("sc://10.0.0.50:15002")
    .getOrCreate())
```
# Submit program to spark
```
spark-submit --master spark://srv-01:7077 /opt/spark/examples/src/main/python/pi.py 
```
