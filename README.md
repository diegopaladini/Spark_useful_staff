# Spark_useful_staff
Tips for spark configuration

HOW TO USE POOL RESOURCES MANAGEMENT IN THE SPARK JOBS ON HADOOP 

java parameters
-Dmapreduce.job.queuename=<QUEUE_NAME>

spark summit parameters
spark-submit   --queue <QUEUE_NAME>
spark.yarn.queue=<QUEUE_NAME>

oozie

<global>
        <configuration>
            <property>
                <name>mapreduce.job.queuename</name>
                <value><QUEUE_NAME></value>
            </property>
        </configuration>
    </global>

	

query	
•	Spark : --queue <QUEUE_NAME> (for example spark-submit   --queue <QUEUE_NAME>)
•	Hive : set mapreduce.job.queuename=<QUEUE_NAME> (add this in your hql script)
•	Impala : SET REQUEST_POOL=<QUEUE_NAME>
•	Oozie : mapreduce.job.queuename
