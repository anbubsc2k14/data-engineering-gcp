### HDFC to Spark RDD:

In this example, we first create a SparkConf object to configure the Spark application with a name of "MyApp" and a master URL of "local". Then, we create a SparkContext object using the SparkConf object.

Next, we use the textFile() method of the SparkContext object to load a text file from HDFS into an RDD. The argument to textFile() is the path to the file on HDFS, in this case "hdfs://localhost:9000/path/to/file".

Finally, we use the collect() method of the RDD to retrieve all the elements of the RDD and print them out one by one using a for loop.

Note that the textFile() method returns an RDD of strings, where each string corresponds to a line in the file. If you need to parse the data in the file into a different format, you'll need to use other methods of the RDD like map() or flatMap().
