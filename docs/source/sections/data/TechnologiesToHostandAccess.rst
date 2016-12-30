**************************************************************
Google Technologies Used to Host Data (and How to Access Them)
**************************************************************
Google has `many technologies <https://cloud.google.com/products/storage/>`_ to store your data.  ISB-CGC has chosen technologies that enable common workflows using historically used file based methods (as the TCGA data exists in the GDC), as well as in `data tools <https://cloud.google.com/products/#big-data>`_ that are well adapted to the speed and extensibility of the cloud ("Big Data").  Overviews are provided below, with links to more specific detailed documentation of how to use it at ISB-CGC.

Google Technologies Used to Host Data
#####################################

ISB-CGC hosts biomedical data in three types of Google Technologies:

- Google Cloud Storage (GCS_) - this is the basic object storage mechanism for rapidly accessing files.  This is where copies of the raw data files at the `Genomic Data Commons <https://gdc.cancer.gov/>`_ are stored for use with ISB-CGC and Google Cloud Platform technologies. These files can be used by the same analytic programs that have been written to handle the raw data files used to analyze TCGA and other genomic and medical data in a non cloud-based computer environment.  This is done by creating a copy on a `persistant disk <https://cloud.google.com/persistent-disk/>`_ store mounted to your virtual machine that you are doing the computations on.
- BigQuery_ - the information scattered over tens of thousands of XML and TSV files at the Genomic Data Commons is provided in a much more accessible form in a series of open-access BigQuery tables.  The high-level (*"Level 3"*) data (described in more detail `here <TCGA-Data.html>`_) are `Extracted, Transformed and Loaded <data2/data_in_BQ.html#etl-details-for-tcga-data>`_ (ETL) into simple summary tables that can be readily used for analysis across ALL TCGA cancer types, without needing to parse the data from 100's of individual files.  Analyses can be done using either standard SQL queries, or by simple modifications of existing analytic programs to pull the relevant data from BigQuery tables (see below for more details).
- `Google Genomics <https://cloud.google.com/genomics/>`_ - new text here

.. _GCS: https://cloud.google.com/storage/
.. _BigQuery: https://cloud.google.com/bigquery/

How to Access Biomedical Data Hosted on ISB-CGC
###############################################
Data can be accessed through both a Graphical User Interface or Programmatically through command lines and programs.  To access data through the Graphical User Interface, specific details on how to find and use the data are handled by ISB-CGC.  Programmatic access is done through well defined Application Programming Interfaces (APIs) that detailed in links provided in the sections below, grouped by Google Technology.

Google Cloud Storage
====================
Text here (optional)

Details of how to find the files of interest
--------------------------------------------
Text here

Details of how to use the files of interest programmatically
------------------------------------------------------------
text here

BigQuery
========
Text here (optional)

Details of how to find the data of interest
-------------------------------------------
text here

Details of how to use the data of interest programmatically
-----------------------------------------------------------
text here

Google Genomics
===============
Text here (optional)

Details of how to find the data of interest
-------------------------------------------
text here

Details of how to use the data of interest programmatically
-----------------------------------------------------------
text here
