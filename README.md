# Apache Hudi Examples

<img width="85" alt="map-user" src="https://img.shields.io/badge/views-797-green"> <img width="125" alt="map-user" src="https://img.shields.io/badge/unique visits-193-green">

Apache Hudi examples designed to be run on AWS Elastic Map Reduce (EMR) via. EMR Studio and/or EMR Notebook(s).

Reference background on key [concepts](https://hudi.apache.org/docs/concepts/). If you are new to working with Hudi it is worth reading about Hudi's [timeline](https://hudi.apache.org/docs/concepts/#timeline), [file management](https://hudi.apache.org/docs/concepts/#file-management), [index](https://hudi.apache.org/docs/concepts/#index), [table types](https://hudi.apache.org/docs/concepts/#table-types), [query types](https://hudi.apache.org/docs/concepts/#query-types), [copy on write](https://hudi.apache.org/docs/concepts/#copy-on-write-table), [merge on read](https://hudi.apache.org/docs/concepts/#merge-on-read-table).

If you are not familiar with the core Hudi concepts or are new to Hudi I **highly** recommend you watch [AWS re:Invent 2019: Insert, upsert, and delete data in Amazon S3 using Amazon](https://www.youtube.com/watch?v=_ckNyL_Nr1A).

## Enviorment Set Up

The samples in this repository are designed to run on EMR via. EMR Notebooks or EMR Studio. To set up your enviorment follow the AWS documentation for [EMR Notebooks](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-managed-notebooks.html) or [EMR Studio](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-studio.html).

You can upload the .ipynb files in this repository directly to the Jupyter enviorments provides by EMR Notebooks / Studio

## Copy on Write
The notebooks in [copy_on_write](https://github.com/ev2900/Hudi_Elastic_Map_Reduce/tree/main/copy_on_write) is the best place to start. It covers working with data via. Hudi specific to **copy on write** tables. The notebook(s) covers
* Writing data to S3
* Reading data from S3
* Upserting data
* Incremental querying
* Point in Time querying
* Deleting Data

Both a [Python](https://github.com/ev2900/Hudi_Elastic_Map_Reduce/blob/main/copy_on_write/Python/copy_on_write_python.ipynb) and [Scala](https://github.com/ev2900/Hudi_Elastic_Map_Reduce/blob/main/copy_on_write/Scala/copy_on_write_scala.ipynb) notebooks are available.

## Merge on Read
The notebook in [merge_on_read](https://github.com/ev2900/Hudi_Elastic_Map_Reduce/tree/main/merge_on_read) is the best next step once you understand the [copy_on_write](https://github.com/ev2900/Hudi_Elastic_Map_Reduce/tree/main/copy_on_write) notebook(s). The [merge_on_read](https://github.com/ev2900/Hudi_Elastic_Map_Reduce/tree/main/merge_on_read) notebook covers
* Writing data to S3
* Upserting data
* Snapshot queries
* Read optimized queries
* Compaction

Both a [Python](https://github.com/ev2900/Hudi_Elastic_Map_Reduce/tree/main/merge_on_read/Python/merge_on_read_python.ipynb) and [Scala](https://github.com/ev2900/Hudi_Elastic_Map_Reduce/tree/main/merge_on_read/Scala/merge_on_read_scala.ipynb) notebooks are available.

## Future Imporvement to this Repo
* Hudi SQL example(s)
* Hudi time travel example(s)
