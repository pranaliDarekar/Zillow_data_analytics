Zillow_data_analytics

In this data engineering project, we will demonstrate how to create an automated Python ETL (Extract, Transform, Load) pipeline. This pipeline will extract real estate property data from the Zillow Rapid API, transform it, and store it in an Amazon S3 bucket. Subsequently, a series of AWS Lambda functions will be triggered to further process the data, including conversion to CSV format, and the data will be loaded into another S3 bucket.

Apache Airflow, an open-source tool, will be used for orchestrating and scheduling these tasks and data pipelines. Specifically, we will use the S3KeySensor operator in Apache Airflow to monitor the availability of transformed data in the AWS S3 bucket before proceeding to load the data into Amazon Redshift, a data warehousing solution.

Once the data is successfully loaded into Amazon Redshift, we will connect Amazon QuickSight to the Redshift cluster to create visualizations of the Zillow Rapid data. This entire project will be executed on the AWS cloud platform.
