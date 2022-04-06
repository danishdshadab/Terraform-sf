# Terraform script to update snowflake

## Prerequisite
1. Snowflake User and password: There need to create a user in snowflake which will have the below access. The User is needed so that terraform can create all required objects.
2. Server to run the terraform: The terraform can be run from the local or EC2. For the given exercise a Linux EC2 server is used.
3. Setup Terraform Authentication: Below are the authentication needed to be setup in terraform environment variable.
	SNOWFLAKE_USER,SNOWFLAKE_PASSWORD,SNOWFLAKE_ACCOUNT,SNOWFLAKE_REGION
  
