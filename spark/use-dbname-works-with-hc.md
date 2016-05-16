# "use <dbname>" works only with HiveContext for spark-submit

The SQL statement to select an existing database schema - use dbname - works only with the HiveContext in code submitted using spark-submit. 
sqlContext.sql("use my_db") results in a parsing exception suggestion "with" to be used instead of "use". However, the same statement on sqlContext works fine on the spark shell. 

TODO: This probably is a bug to be filed. 

 
