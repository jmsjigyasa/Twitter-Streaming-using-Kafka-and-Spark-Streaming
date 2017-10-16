Real time streaming and sentiment analysis of twitter data using kafka and pyspark

Note: We are using Python 2.7 version, Also when downloading kafka and spark don't go for the latest version download atleast one year old release.

In this repo we are creating a pipeline to stream tweets from twitter using tweepy library and making it as a producer for kafka and then making the pyspark as the consumer to fetch the tweets get the do sentiment analysis on the tweets. Find the steps below to start your ownn sstreaming application.

Download kafka from https://www.apache.org/dyn/closer.cgi?path=/kafka/0.11.0.1/kafka_2.11-0.11.0.1.tgz
Untar kafka and then using cmd cd into the folder that got created after untaring it
Execute the first three commands in the script.txt file. Note: each command will be executed on different cmd and dont close the cmd
Download the python file tweetkafka.py from the repo and run it it will start producing messages on Kafka
Download spark from https://spark.apache.org/downloads.html. I used the 2.0.0 version for this experiment
After you untar the spark cd inside that folder and create a directory called hadoop\bin
Download winutils.exe for hadoop version 2.7 and put it inside the spark\hadoop\bin folder
Create SPARK_HOME system variable pointing to your spark directory and HADOOP_HOME system variable pointing to spark\hadoop\bin folder
Do pip install nltk and pip install vaderSentiment for sentiment analysis (Note it is for Python version 2.7)
For more info on vadersentiment follow the link :https://github.com/cjhutto/vaderSentiment
put the file constest.py from the repo inside the spark folder
execute python constest.py from cmd and it will start your pipeline.
Thank you
