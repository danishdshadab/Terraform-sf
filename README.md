# Terraform script to update snowflake

## SNOWWACTH intro

Snowwatch is an application which monitors the snowflake Usage on below metrics.
1. Warehouse Credit -> It enables user to access the credit usage on user and Roles level.
		  like which users/role has been using the most credit on day to day level.
2. Storage credit -> It enables the user to monitor the credit usage of used and unused storage.
          like users can get access of dummy/unused tables which are not used from last one month etc.
3. Roles and users access -> Enables users to monitor the Roles and Users created on the account.
          The metrics can be used for audit and governance puprose. It can be used to view the the unused users, Roles and grants.

## Prerequisite

Terraform User and password: Create a user in snowflake which will be used to run the terraform script. for snowwatch application the User should have role with following privilege. Create Database,Schema, tables and task

Server to run the terraform: The terraform can be run from the local or EC2. For the given exercise a Linux EC2 server is used.

Setup Terraform Authentication: Below are the authentication needed to be setup in terraform environment variable. 
```
export SNOWFLAKE_ACCOUNT="XXXXXXXXXXXXXXXXXX"
export SNOWFLAKE_USER="XXXXXXXXXX"
export SNOWFLAKE_PASSWORD="XXXXXXXXXXX"
```
 
