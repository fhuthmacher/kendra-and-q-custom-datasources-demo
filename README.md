# kendra-and-q-custom-datasources-demo
Walkthrough of custom data source set up for Amazon Kendra and Amazon Q

## Overview

This repository contains several notebooks that walk through the setup of 
a) custom data sources for Amazon Kendra and Amazon Q
b) S3 data source for Amazon Kendra
c) Search with Amazon Kendra & ChatSync with Amazon Q

## Getting started

1. Clone the repository

   ```
   git clone https://github.com/fhuthmacher/kendra-and-q-custom-datasources-demo.git
   cd kendra-and-q-custom-datasources-demo
   ```

2. Set up a virtual environment

   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install dependencies

   ```
   pip install -r requirements.txt
   ```

4. Set the environment variables in dev.env
Update the below environment variables.

    ```
    REGION=us-east-1
    KENDRA_INDEX=XXX
    KENDRA_ROLE=XXX
    AMAZON_Q_APP_ID=XXX
    DEMO_S3_BUCKET=XXX
    DEMO_S3_KEY=XXX
    CLOUDFRONT_URL=XXX
    ```

5. Explore the notebooks
- 01_CustomConnector.ipynb : Covers the setup of custom data sources for Amazon Kendra and Amazon Q
- 02_CreateS3DataSourcewithACL.ipynb : Creates S3 data source for Amazon Kendra with ACL
- 03_Search.ipynb : Explores a couple of Kendra Search and Q Business examples

## Authors

- Felix Huthmacher  - *Initial work* - [github](https://github.com/fhuthmacher)

## References

- Refer to https://github.com/aws-samples/configuring-qbusiness-with-idc-tti/tree/main for detailed instructions and examples on QBusiness authentication setup with various different IdPs.