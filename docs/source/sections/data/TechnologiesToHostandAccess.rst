**************************************************************
Google Technologies Used to Host Data (and How to Access Them)
**************************************************************
Google has `many technologies <https://cloud.google.com/products/storage/>`_ to store your data.  ISB-CGC has chosen technologies that enable common workflows using historically used file based methods (as the TCGA data exists in the GDC), as well as in `data tools <https://cloud.google.com/products/#big-data>`_ that are well adapted to the speed and extensibility of the cloud ("Big Data").  Overviews are provided below, with links to more specific detailed documentation of how to use it at ISB-CGC.

Google Technologies Used to Host Data
#####################################

ISB-CGC hosts biomedical data in three types of Google Technologies:

- Google Cloud Storage (GCS_) - this is the basic object storage mechanism for rapidly accessing files.  This is where copies of the raw data files at the `Genomic Data Commons <https://gdc.cancer.gov/>`_ are stored for use with ISB-CGC and Google Cloud Platform technologies. These files can be used by the same analytic programs that have been written to handle the raw data files used in a non-cloud based computer environment.  This is done by creating a copy on a `persistant disk <https://cloud.google.com/persistent-disk/>`_ store mounted to your virtual machine that you are doing the computations on.
- BigQuery_ - new text here
- `Google Genomics <https://cloud.google.com/genomics/>`_ - new text here

.. _GCS: https://cloud.google.com/storage/
.. _BigQuery: https://cloud.google.com/bigquery/

How to Access Biomedical Data Hosted on ISB-CGC
###############################################
- Google Cloud Storage
 - Details of how to find the files of interest.
 - Details of how to use the files of interest programmatically
- BigQuery
 - Details of how to find the data of interest.
 - Details of how to use the data of interest programmatically
-Google Genomics
 - Details of how to find the data of interest.
 - Details of how to use the data of interest programmatically
