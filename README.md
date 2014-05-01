Trade Sequence
==============

This project demonstrates how to process time-series data using [Apache Crunch](http://crunch.apache.org/index.html) using the simple example of sequencing trades for each stock by time.

Running
-------

The compiled program can be run on a Hadoop cluster with:

`hadoop jar target/tradesequence-0.0.1-SNAPSHOT-job.jar /hdfs/input/directory /hdfs/output/directory`

Test data
---------

A small test data JSON file is provided in `src/main/avro`. On a CDH5 cluster it can be converted to an Avro file using `src/main/avro/create_test_avro.sh`. On another Hadoop distribution you can alter the script to point to your avro-tools location. The Avro data file can be used as the input for the job.
