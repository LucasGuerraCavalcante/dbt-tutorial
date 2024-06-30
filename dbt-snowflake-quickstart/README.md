Welcome to your new dbt project!

### Using the starter project

Try running the following commands:
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](https://community.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices


# dbt Project Setup Guide

This guide will walk you through the steps to set up a dbt project that uses Snowflake as the data warehouse. The project will include a model that is built using a sample query, tests for the model, and documentation.

## Prerequisites

Before you begin, you should have the following:

- A Snowflake account
- Access to dbt Cloud
- Basic knowledge of SQL

## Step 1: Create a new Snowflake worksheet

Log in to your Snowflake account and create a new worksheet. This will be used to run queries and create tables.

## Step 2: Load sample data into your Snowflake account

Download the sample data from the public S3 bucket and load it into your Snowflake account. This data is stored as CSV files, so you can use the `COPY INTO` command to load it into Snowflake.

## Step 3: Connect dbt Cloud to Snowflake

Create a new project in dbt Cloud and connect it to your Snowflake account. This will allow you to run dbt commands and deploy your models to Snowflake.

## Step 4: Create a dbt model

Take a sample query and turn it into a model in your dbt project. A model in dbt is a select statement. You can use the `{{ ref('table_name') }}` syntax to reference other tables in your query.

## Step 5: Add tests to your models

Add tests to your models to ensure that they are working as expected. You can use the `assert*` macros provided by dbt to write tests that check the output of your models.

## Step 6: Document your models

Document your models using the `description` field in the `models.yml` file. This will provide context for other users who may need to work with your models in the future.

## Step 7: Schedule a job to run

Schedule a dbt job to run on a regular basis. This will ensure that your models are kept up-to-date with the latest data in your Snowflake account.

And that's it! You now have a fully-functional dbt project that uses Snowflake as the data warehouse.
