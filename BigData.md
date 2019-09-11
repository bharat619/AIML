## Rise of bytes
We are in exabyte 1000^6 EB -> Exabytes
Yet to reach -> Zetabyte (1000^7 ZB) and Yotabyte(1000^8 YB)

## Types of data
- Structured data ( sitting in form of rows and columns (RDBMS) )
- Semi structured data ( Any data that does not fit in rows and columns but fit into RDBMS table, (XML) )
- Unstructured data ( data which can never fit into rows and columns of RDBMS ex: email body, text messages, server logs )

semi structured data example: email
Email body is candidate for unstructured data
But email has head and body, like a header and footer. This fits into a semi structured data

## Big Data
Buzzword used to term massive amount of data originating from structured and unstructured source which is very large and complex to process using existing database and software techniques

Data originates from
- Human originated data
  - Blogs ,Reviews, Emailss, Scientific Research
  - Social graphs: Facebook, Twitter, LinkedIn, Contacts
- Machine generated data
  - Sensor data, Cellphone data, geospatial data,
  - application server logs

## Why Big Data is important
1. Manage and process huge amount of data cost efficiently
2. Analyse data in all forms (structured, semi, unstruct)
3. captures data from fast happening source
4. handles failures of node and task assigned to them
5. turn data into measurable insights

## Characteristics of Big Data
 - Volume
 - Velocity: Rate at which data is generated
 - Variety: 80% of data is unstructured
 - Veracity: Uncertainity in correctness of data because of ambiguity, inconsistency or latency
 - Variability: Inconsistency in flow of data. Example: 2 temprature measuring devices might be slight varied in their data recordings
 - Value: Extracting business value and insights

## Challenges of Big data
1. Cost
2. Scalability
3. Handling variety of data
4. Processing huge data
5. Storing huge size of data


## Open source for big data
Hadoop, spark

## Hadoop
- General purpose OS like framework for parallel processing
- Open source
- Since its free, mid sized organisation are able to open up cluster

## Architecture of Hadoop
Hadoop V1:
- Machines in Master mode(Name node, Secondary name node and job tracker) are inter connected with data nodes in slave mode

Deployment of Hadoop:
(Services in below points refer name node, secondary name node and job tracker node)
- Supports 3 configuration modes
  1. Standalone mode: All services run locally on single machine on a single JVM
  2. Pseudo distributed mode: All services run on same machine but on different JVM container ( development and testing purpose)
  3. Fully distributed mode: Each service runs on a separate hardware. ( production)

## Functionality of each component in Hadoop
- Name node:
  -Central file system manager
  -Saves file into multiple data nodes
  -Splits into multiple blocks, and is pushed into the data nodes
  - Doesn't store the file, but knows the location of where exactly the file resides
- Secondary name node:
  - Backup of the name node
  - In hadopp v2 name node has hot standby name node
- Job tracker
  - centralised job scheduler

- Data node:
  - file is stored and actual data processing happens
- Task tracker
  a software  service which monitors state of job tracker

Slave nodes keeps sending heart beat signal to master every 3 seconds to state its alive

## JOB in Hadoop system
Task submitted by user to hadoop system
Job is a collection of program in the cluster

Job consists of
   - JAR File
   - Input file path and output file path

## Apache Hadoop core features
- Hadoop Distributed File System (HDFS) - data storage
- MapReduce Framework - parallel processing framework

## Submitting a job to hadoop cluster
