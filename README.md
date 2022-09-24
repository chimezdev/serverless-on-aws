# serverless-on-aws
The file 'index-mock.js' is for creating a serverless application using lambda function with mock data.

# steps
# create a lambda function
- Create a default lambda function on aws
- Copy the code in the 'index-mock.js' file and replace the default lambda code with it.
- Redeploy the function

# create a REST API on aws
Go to the api gateway console on aws 
click on 'BUILD' of the REST API type
Click on the radio button to select 'REST' and 'New API'
Give the api a name, description. Select 'Edge optimized as Endpoint Type and click to create.
- Click on 'Actions' and select 'Create resources', provide the resource name in this case 'groups'. This is the path parameter endpoint.

# Creating a lambda function that gets resources from a database (dynamoDB)

# Steps
# Creating DynamoDB database
- Navigate to the dynamodb console on aws and click on 'Create Table
Provide table name, partition key-this is compulsory, use id and select type string
Select 'customize setting' and select 'DynamoDB Standard'
Select 'On-demand' under 'Read/Write capacity settings.
Leave the other settings as default and click to create.

# Populate the created table with data.
Select the created table and click on 'action' - 'create items'
