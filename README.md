## CDHBDRAutomation

Automation to build an operational DR using Cloudera Hadoop Distribution

### Introduction

This is a tool to automate your CDH BDR setup. If you want to use CDH BDR(https://www.cloudera.com/documentation/enterprise/5-9-x/topics/cm_bdr_tutorials.html) to build your DR you would definately feel the tool though self sufficient but still it needs few fine include you in your complaint enterprise environment.

***Below are the features that is missing in BDR working alone:***
  1. Scheduling BDR jobs using your enterprise scheduling tool.
  2. Customised alerting for Job status.
  3. BDR Job probing and detect hung/failed condition.
  4. Avoid considering obvious FileNotFound error and a failure as most often it is generated by temporary files.
  5. No historical job log cleanup feature present in BDR at this point.

This is exactly where this tool comes into picture. Its build to make BDR your enterprise ready. 

***Below are the major features:***
  1. Schedule your BDR Replication job using your scheduler rather than CM itself.
  2. It doesnot consider FileNotFound error as a failer BDR execution though it reports the same via mail with exact files which failed to be replicated.
  3. Hung detection logic inbuild thus you get status of job in definite fashion.
  4. Custom alerting mechanism.
  5. Supplimentary Cleanup tool to clean up ever growing BDR Job logs created in HDFS.
  
### Setup and Configuration

The tool does not need any setup requirement just coping the same to any location from where your scheduler can execute the same. Since the tool is written for Unix environment thus bash shell is a requirement. Also do remember the tool make API call to CM thus should have connectivity for the same.

In addition to the above the configuration file need to be completed with appropiate value suitable for your environment. The file is faily well comment for your understanding.

### Support and managebility

If you are reading this README file then you are probably about to use the my tools to help you complete your BDR setup. Good choice. This tool is made for you. Moreover this tool is free and always will be thats my promise.

Now it is hard to believe that you will get 24/7 Support thats too much to ask for. But in case you face any issue and want my intervention and you cannot debug the hundreeds lines of core Bash Script your self, please do not hassitate to write to me. Its a guarentee you will get an answer but it is not a guarentee you will have it in a SLA.

Reach Me: sanmuk21@gmail.com

Best of luck. Happy building successful DR for your CDH Hadoop Cluster.
