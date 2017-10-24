# Spark_useful_staff
Tips for spark configuration

HOW TO USE POOL RESOURCES MANAGEMENT IN THE SPARK JOBS ON HADOOP 

java parameters
-Dmapreduce.job.queuename=queue_name

spark summit parameters
spark-submit   --queue axa_italy
spark.yarn.queue=axa_italy

oozie

<global>
        <configuration>
            <property>
                <name>mapreduce.job.queuename</name>
                <value>${queueName}</value>
            </property>
        </configuration>
    </global>

	

query	
•	Spark : --queue axa_italy (for example spark-submit   --queue axa_italy)
•	Hive : set mapreduce.job.queuename=axa_italy (add this in your hql script)
•	Impala : SET REQUEST_POOL=(add this in your sql script)
•	Oozie : mapreduce.job.queuename
