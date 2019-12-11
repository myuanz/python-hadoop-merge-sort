"# python-hadoop-merge-sort" 

hadoop build with Docker-compose, write in Python.
Building reference here: https://github.com/big-data-europe/docker-hadoop

result: 
```
root@7a1f9c75ca15:~/hadoop-test# ./run.sh
Deleted /root/hadoop-test
2019-12-11 05:52:48,020 INFO sasl.SaslDataTransferClient: SASL encryption trust check: localHostTrusted = false, remoteHostTrusted = false
Deleted /output
2019-12-11 05:52:50,612 WARN streaming.StreamJob: -file option is deprecated, please use generic option -files instead.
packageJobJar: [./mapper.py, ./reducer.py, /tmp/hadoop-unjar3228496350451081237/] [] /tmp/streamjob5140522774046212296.jar tmpDir=null
2019-12-11 05:52:51,337 INFO client.RMProxy: Connecting to ResourceManager at resourcemanager/172.20.0.4:8032
2019-12-11 05:52:51,469 INFO client.AHSProxy: Connecting to Application History server at historyserver/172.20.0.2:10200
2019-12-11 05:52:51,493 INFO client.RMProxy: Connecting to ResourceManager at resourcemanager/172.20.0.4:8032
2019-12-11 05:52:51,494 INFO client.AHSProxy: Connecting to Application History server at historyserver/172.20.0.2:10200
2019-12-11 05:52:51,633 INFO mapreduce.JobResourceUploader: Disabling Erasure Coding for path: /tmp/hadoop-yarn/staging/root/.staging/job_1576027383119_0034
2019-12-11 05:52:51,727 INFO sasl.SaslDataTransferClient: SASL encryption trust check: localHostTrusted = false, remoteHostTrusted = false
2019-12-11 05:52:51,800 INFO sasl.SaslDataTransferClient: SASL encryption trust check: localHostTrusted = false, remoteHostTrusted = false
2019-12-11 05:52:51,824 INFO sasl.SaslDataTransferClient: SASL encryption trust check: localHostTrusted = false, remoteHostTrusted = false
2019-12-11 05:52:51,874 INFO mapred.FileInputFormat: Total input files to process : 1
2019-12-11 05:52:51,896 INFO sasl.SaslDataTransferClient: SASL encryption trust check: localHostTrusted = false, remoteHostTrusted = false
2019-12-11 05:52:51,911 INFO sasl.SaslDataTransferClient: SASL encryption trust check: localHostTrusted = false, remoteHostTrusted = false
2019-12-11 05:52:51,917 INFO mapreduce.JobSubmitter: number of splits:2
2019-12-11 05:52:52,008 INFO sasl.SaslDataTransferClient: SASL encryption trust check: localHostTrusted = false, remoteHostTrusted = false
2019-12-11 05:52:52,025 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1576027383119_0034
2019-12-11 05:52:52,026 INFO mapreduce.JobSubmitter: Executing with tokens: []
2019-12-11 05:52:52,149 INFO conf.Configuration: resource-types.xml not found
2019-12-11 05:52:52,150 INFO resource.ResourceUtils: Unable to find 'resource-types.xml'.
2019-12-11 05:52:52,397 INFO impl.YarnClientImpl: Submitted application application_1576027383119_0034
2019-12-11 05:52:52,431 INFO mapreduce.Job: The url to track the job: http://resourcemanager:8088/proxy/application_1576027383119_0034/
2019-12-11 05:52:52,433 INFO mapreduce.Job: Running job: job_1576027383119_0034
2019-12-11 05:52:56,495 INFO mapreduce.Job: Job job_1576027383119_0034 running in uber mode : false
2019-12-11 05:52:56,496 INFO mapreduce.Job:  map 0% reduce 0%
2019-12-11 05:53:01,537 INFO mapreduce.Job:  map 50% reduce 0%
2019-12-11 05:53:02,542 INFO mapreduce.Job:  map 100% reduce 0%
2019-12-11 05:53:05,557 INFO mapreduce.Job:  map 100% reduce 100%
2019-12-11 05:53:05,565 INFO mapreduce.Job: Job job_1576027383119_0034 completed successfully
2019-12-11 05:53:05,626 INFO mapreduce.Job: Counters: 53
        File System Counters
                FILE: Number of bytes read=134
                FILE: Number of bytes written=673620
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=489
                HDFS: Number of bytes written=233
                HDFS: Number of read operations=11
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=2
        Job Counters
                Launched map tasks=2
                Launched reduce tasks=1
                Rack-local map tasks=2
                Total time spent by all maps in occupied slots (ms)=15052
                Total time spent by all reduces in occupied slots (ms)=13424
                Total time spent by all map tasks (ms)=3763
                Total time spent by all reduce tasks (ms)=1678
                Total vcore-milliseconds taken by all map tasks=3763
                Total vcore-milliseconds taken by all reduce tasks=1678
                Total megabyte-milliseconds taken by all map tasks=15413248
                Total megabyte-milliseconds taken by all reduce tasks=13746176
        Map-Reduce Framework
                Map input records=17
                Map output records=17
                Map output bytes=194
                Map output materialized bytes=149
                Input split bytes=198
                Combine input records=0
                Combine output records=0
                Reduce input groups=14
                Reduce shuffle bytes=149
                Reduce input records=17
                Reduce output records=1
                Spilled Records=34
                Shuffled Maps =2
                Failed Shuffles=0
                Merged Map outputs=2
                GC time elapsed (ms)=134
                CPU time spent (ms)=1110
                Physical memory (bytes) snapshot=722718720
                Virtual memory (bytes) snapshot=18622185472
                Total committed heap usage (bytes)=609746944
                Peak Map Physical memory (bytes)=279285760
                Peak Map Virtual memory (bytes)=5095006208
                Peak Reduce Physical memory (bytes)=169390080
                Peak Reduce Virtual memory (bytes)=8437309440
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=291
        File Output Format Counters
                Bytes Written=233
2019-12-11 05:53:05,626 INFO streaming.StreamJob: Output directory: /output
2019-12-11 05:53:07,104 INFO sasl.SaslDataTransferClient: SASL encryption trust check: localHostTrusted = false, remoteHostTrusted = false
[1, 1, 1, 2, 2, 2, 2, 3, 4, 5, 5, 5, 6, 7, 7, 7, 8, 8, 8, 13, 23, 23, 34, 34, 35, 35, 35, 52, 123, 124, 135, 234, 234, 235, 235, 235, 235, 
235, 235, 235, 236, 253, 412, 421, 423, 512, 512, 523, 1235, 2345, 2356, 3521, 23456, 24356]
```