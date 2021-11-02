Execute word count using HappyBase in VS:

Hadoop version -3.3.1
Hbase version -1.4.6

Step 1:
pip3 install happybase

Step 2:
Start hadoop,hbase daemons start happybase daemon
start-all.sh
start-hbase.sh
hbase-daemon.sh start thrift

Step 3:
Copy the word count program output to our program folder and convert that to csv file.
And give columns names in that file.
$ hdfs dfs -get /WordCountHBase/Output /home/namratha/Documents

Step 4:
Write python code by using happybase library to:
* Create a table.
* Put the output data into the table.
* Display that data in the table.

Step 5:
Verify the data in hbase shell
scan 'word_count'
