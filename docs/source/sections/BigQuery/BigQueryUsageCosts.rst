*************
 Usage Costs 
*************

There are two basic types of usages costs associated with BigQuery: **query costs** and **storage costs**. 

Query Costs
-----------

The main costs associated with using BigQuery are the query costs.  In BigQuery, queries are billed according to how much data is scanned during the course of the query, and the rate is $5 per TB, although the first **1 TB is free each month**. Queries can be more expensive as they become more computationally intensive.  

While most of the cost is suprisingly low, it is always important to think carefully about your queries and to make them as efficient as possible.  For example, if you want to derive summary information about all ~20,000 genes, you could do that with a single query that might cost a few pennies, or you might write a less-clever query that returns information only about a single gene and then programmatically loop over all genes, running that single-gene query 20,000 times. Your overall query costs using this less-clever approach, instead of being a few pennies would be several hundred dollars!  This latter approach would also take significantly more time.


Storage Costs
------------

You want to upload your own data to BigQuery or to store results of your queries as new BigQuery tables. In BigQuery, storage costs are based on the amount of data stored. For example, ISB-CGC is hosting PanCancer Atlas tables in BigQuery and is paying for the storage costs (with support from NCI). The size of each PanCancer Atlas table is less than 1.5 GB and therefore costs less than $0.25 per year to store. 

The image below summarizes BigQuery's storage costs (as of August 2019). Note, these prices are subject to change so check  Google's pricing page, https://cloud.google.com/bigquery/pricing for the most up-to-date costs. 

.. image:: BigQueryCosts.png
   :scale: 50
   :align: center

 



Additional Support
-----------------
Latest information about BigQuery can be found here:  https://cloud.google.com/bigquery 

Some more helpful links:
=======================

`Introductory Information from Google <https://cloud.google.com/bigquery/what-is-bigquery>`_

`Main Google BigQuery documentation <https://cloud.google.com/bigquery/docs>`_

`QuickStart Guide <https://cloud.google.com/bigquery/docs/quickstarts/quickstart-web-ui>`_

`Query Syntax <https://cloud.google.com/bigquery/query-reference>`_

`Detailed information on Google pricing <https://cloud.google.com/bigquery/pricing>`_

`Estimating storage and query costs <https://cloud.google.com/bigquery/docs/estimate-costs>`_

`Best practices on how to control costs <https://cloud.google.com/bigquery/docs/best-practices-costs>`_

`Keep an eye on your GCP expenses on your Google Cloud Platform Console home page <https://console.cloud.google.com/home/dashboard>`_

`BigQuery Mate Chrome Web Extenstion <https://chrome.google.com/webstore/detail/bigquery-mate/nepgdloeceldecnoaaegljlichnfognh?hl=en-US>`_


