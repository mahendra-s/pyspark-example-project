### Set spark and pyspark
```
set spark_home=C:\Users\Mahendra\AppData\Local\spark-2.4.8-bin-hadoop2.7
set hadoop_home=C:\Users\Mahendra\AppData\Local\spark-2.4.8-bin-hadoop2.7 
```
### set python 
```
set python_home=C:\Users\Mahendra\AppData\Local\Programs\Python\Python36
set pythonpath=%SPARK_HOME%\python;%SPARK_HOME%\python\lib\*.zip;%PYTHONPATH%
```
### run example from home directory 
```
%SPARK_HOME%\bin\spark-submit  --master local[*]   --py-files packages.zip  --files configs\etl_config.json  jobs\etl_job.py
```