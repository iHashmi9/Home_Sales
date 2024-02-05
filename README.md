Initial Import Dependencies pulled from class instructions from Professor Seeber

Structure of the csv was verified using pyspark.sql.types 

Following temporary view was used to create the view:
"spark.sparkContext.addFile(url)
file_path = "file://" + SparkFiles.get("home_sales_revised.csv") with the aid of ChatGPT
df = spark.sql(f"SELECT * FROM csv.`{file_path}`")
df.createOrReplaceTempView("home_sales")"

Schema was verified and changed to the following types:
in this order: Float, Date, Date, Integer, Integer, Integer, Integer, Integer, Integer, Integer, Integer

Schema change script was pulled from chatgpt and lectures

Spark.SQL code was verified using chatgpt

Table Cached check process was pulled from chatgpt
