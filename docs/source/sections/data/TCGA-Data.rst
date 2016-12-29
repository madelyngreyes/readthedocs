*******************
About the TCGA Data
*******************

The ISB-CGC hosts approximately 1 petabyte of TCGA_ data in various Google Cloud Technologies (see this page for more details). 

.. _TCGA: http://cancergenome.nih.gov/
.. _GCS: https://cloud.google.com/storage/
.. _BigQuery: https://cloud.google.com/bigquery/

The vast majority (over 99%) of this **petabyte** of data consists of low-level sequence data, currently stored as files in
Google Cloud Storage.  Over the course of the TCGA project, this low-level (*"Level 1"*) data has been processed through 
a set of standardized pipelines and the the resulting high-level (*"Level 3"*) data is frequently the data that is used
in most downstream analyses.  The figure below summarizes the distribution of the data by both Size of Data as well as Number of Data Files.

.. image:: new-block-three-p.png
   :scale: 100
   :align: center

The ISB-CGC platform aims to make these different types of data accessible to the widest
possible variety of users within the cancer research community, using the most appropriate Google Cloud Platform 
technologies.

More details about the TCGA data-generating platforms, data-types, and levels and can be found in the sections below:

.. toctree::
   :maxdepth: 1

   data2/TCGA_Data_Platforms
   data2/TCGA_Data_Types
   data2/TCGA_Data_Levels

In addition, we recommend that you review important information about data security and data access
in these sections:

.. toctree::
   :maxdepth: 1

   data2/TCGA_Data_Security
   data2/TCGA_Access

And finally, links to useful data reports can be found in this final section:

.. toctree::
   :maxdepth: 1

   data2/TCGA_Reports

