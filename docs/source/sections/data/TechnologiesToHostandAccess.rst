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
Data can be accessed through both a `Web Interface <../Web-UI.html>`_ or Programmatically through command lines and programs.  To access data through the Web Interface, specific details on how to find and use the data are handled by ISB-CGC.  Programmatic access is done through well defined Application Programming Interfaces (APIs) that are detailed in links provided in the sections below, grouped by Google Technology.

Google Cloud Storage
====================
ISB-CGC data stored in GCS is both in open data stores (freely accessible with only a Google ID and a Google Cloud Project necessary to access), or controlled access data stores (requiring a `dbGaP authorization and an NIH ID authentication <../webapp/Gaining-Access-To-TCGA-Contolled-Access-Data.html>`_).

Details of how to find the files of interest
--------------------------------------------
To query and find the location of the data files, use  `ISB-CGC API (v2) <../progapi/Programmatic-API.html#id4>`_.   They can be accessed either through a `Google web interface <https://apis-explorer.appspot.com/apis-explorer/?base=https%3A%2F%2Fapi-dot-isb-cgc.appspot.com%2F_ah%2Fapi#p/isb_cgc_api/v2/>`_, or through `ISB-CGC APIs <../progapi/Programmatic-API.html#isb-cgc-api>`_ that are used on the command line or within programs to access the information.  Groupings of patients and samples ("cohorts", a concept central to ISB-CGC) can be created in the Web Interface and used programmatically, or created programmatically and used in the Web Interface, as explained in detail `here <../webapp/ViewingCohorts.html>`_.

Details of how to use the files of interest programmatically
------------------------------------------------------------
We have both `R and Python Tutorials <../progapi/Tutorials.html>`_ showing examples of how to perform customized analyses with ISB-CGC data using our APIs.

*PLEASE NOTE*: other programming languages can easily be used to access the APIs by referencing details in Google's `APIs and Reference documentation <https://cloud.google.com/storage/docs/apis>`_.

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
