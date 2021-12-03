# Apache Hudi Examples
Apache Hudi examples designed to be run on AWS Elastic Map Reduce (EMR) via. EMR Studio and/or EMR Notebook(s).

Youtube video(s)
1. [Hudi Key Concepts][15]
2. Running the Copy of Write example notebook
3. Running the Merge on Read example notebook

Also please reference background on key [concepts][1]. If you are new to working with Hudi it is worth reading about Hudi's [timeline][2], [file management][3], [index][4], [table types][5], [query types][6], [copy on write][7], [merge on read][8].

If you are not familiar with the core Hudi concepts or are new to Hudi I **highly** recommend you watch [AWS re:Invent 2019: Insert, upsert, and delete data in Amazon S3 using Amazon][15].

## Enviorment Set Up

The samples in this repository are designed to run on EMR via. EMR Notebooks or EMR Studio. To set up your enviorment follow the AWS documentation for [EMR Notebooks][10] or [EMR Studio][11]. 

You can upload the .ipynb files in this repository directly to the Jupyter enviorments provides by EMR Notebooks / Studio

## Copy on Write
The notebooks in [copy_on_write][9] is the best place to start. It covers working with data via. Hudi specific to **copy on write** tables. The notebook(s) covers
* Writing data to S3 
* Reading data from S3
* Upserting data
* Incremental querying
* Point in Time querying
* Deleting Data

Both a [Python][12] and [Scala][13] notebooks are available.
## Merge on Read

The notebook in [merge_on_read][14] is the best next step once you understand the [copy_on_write][9] notebook(s). The [merge_on_read][14] notebook covers
* Writing data to S3
* Upserting data
* Snapshot queries
* Read optimized queries
* Compaction

Both a [Python][16] and [Scala][17] notebooks are available.

## Future Improvements Planned for this Repository
* Youtube video - Running the Copy of Write example notebook
* Youtube video - Merge on Read example notebook
* Code samples using Hudi v0.8.0

[1]:https://hudi.apache.org/docs/concepts/
[2]:https://hudi.apache.org/docs/concepts/#timeline
[3]:https://hudi.apache.org/docs/concepts/#file-management
[4]:https://hudi.apache.org/docs/concepts/#index
[5]:https://hudi.apache.org/docs/concepts/#table-types
[6]:https://hudi.apache.org/docs/concepts/#query-types
[7]:https://hudi.apache.org/docs/concepts/#copy-on-write-table
[8]:https://hudi.apache.org/docs/concepts/#merge-on-read-table
[9]:https://github.com/ev2900/Hudi_Elastic_Map_Reduce/tree/main/copy_on_write
[10]:https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-managed-notebooks.html
[11]:https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-studio.html
[12]:https://github.com/ev2900/Hudi_Elastic_Map_Reduce/blob/main/copy_on_write/Python/Hudi%20v0.7.0
[13]:https://github.com/ev2900/Hudi_Elastic_Map_Reduce/blob/main/copy_on_write/Scala/Hudi%20v0.7.0
[14]:https://github.com/ev2900/Hudi_Elastic_Map_Reduce/tree/main/merge_on_read
[15]:https://www.youtube.com/watch?v=_ckNyL_Nr1A
[16]:https://github.com/ev2900/Hudi_Elastic_Map_Reduce/tree/main/merge_on_read/Python/Hudi%20v0.7.0
[17]:https://github.com/ev2900/Hudi_Elastic_Map_Reduce/tree/main/merge_on_read/Scala/Hudi%20v0.7.0
