Execute Live Stock Data using HappyBase in VS:

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
Write python code by using happybase library to:
* Create a table.
* Put the output data into the table.
Download CSV file from : 'https://www.alphavantage.co/query?function=TIME_SERIES_INTRADAY_EXTENDED&symbol=IBM&interval=15min&slice=year1month1&apikey= key'
* Display that data in the table.

Step 4:
Verify the data in hbase shell
scan 'stock'
