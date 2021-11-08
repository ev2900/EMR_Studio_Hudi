# Apache Hudi Examples
Apache Hudi examples designed to be run on AWS Elastic Map Reduce (EMR) via. EMR Studio and/or EMR Notebook(s).

Important background on key [concepts][1]. If you are new to working with Hudi it is worth reading about Hudi's [timeline][2], [file management][3], [index][4], [table types][5], [query types][6], [copy on write][7], [merge on read][8]

## Enviorment Set Up

The samples in this repository are designed to run on EMR via. EMR Notebooks or EMR Studio. To set up your enviorment follow the AWS documentation for [EMR Notebooks][10] or [EMR Studio][11]. 

You can upload the .ipynb files in this repository directly to the Jupyter enviorments provides by EMR Notebooks / Studio

## Getting Started
Notebook [```getting_started.ipynb```][9] is the best place to start. It covers working with data via. Hudi specific to **copy on write** tables. The notebook covers
* Writing data to S3 
* Reading data from S3
* Upserting data
* Incremental querying
* Point in Time querying
* Deleting Data

## Merge on Read

Under development ... I am working on building a similar example to the [```getting_started.ipynb```][9] using merge on read tables. I am working on building out this sample

[1]:https://hudi.apache.org/docs/concepts/
[2]:https://hudi.apache.org/docs/concepts/#timeline
[3]:https://hudi.apache.org/docs/concepts/#file-management
[4]:https://hudi.apache.org/docs/concepts/#index
[5]:https://hudi.apache.org/docs/concepts/#table-types
[6]:https://hudi.apache.org/docs/concepts/#query-types
[7]:https://hudi.apache.org/docs/concepts/#copy-on-write-table
[8]:https://hudi.apache.org/docs/concepts/#merge-on-read-table
[9]:https://github.com/ev2900/Hudi_Elastic_Map_Reduce/blob/main/getting_started/Hudi%20v0.7.0/getting_started.ipynb
[10]:https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-managed-notebooks.html
[11]:https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-studio.html
