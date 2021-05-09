### Serverless Labmda

Not actually serverless, it is just that you do not have to manage your own servers. Directly write code as functions.

### RDS

A database instance. Amazon's rdbms. Can't see tables only storage. For querying tables and stuff, use MySQL workbench.

### Login

Login as root user. (Not IAM user)

### Deployment

Go to S3 under Services.

See Storage, Click on the code/link.

Replace File or Upload new one.

Click deploy.

Note : Change are usually deployed in 24 hours, figure out how to edit metadata to show changes immidieately.

### Layer in Aws

https://www.freecodecamp.org/news/lambda-layers-2f80b9211318/

For importing any library need to add a layer.

Every resource is identifiable via ARN. Copy Paste ARN for adding layer.

aws-sdk included in all.

mysql is also included by default.

### Creating a new function

Create Function.

Author from scratch.

Execution role. (Enable role) [Use an existing role]

VPC - Private network. [1a, 1b enable this]

Security Groups - [enable both]

Click create function.

### Nodejs related stuff

All code in exports handler.

Input will be in `event`. This is the response from the client.

### Response for request in Lambda

Lambda strict with the response u send, exact format of the response connection parameters need to be defined. 

aws doesn’t accept anything which is not json. So, in test event define a JSON.

### Testing

Deploy changes. Go to Test.

Go to cloud watch in services.

Log Groups - Two execution logs. Lambda and API. 

### How to expose the API endpoint

Go to API Gateway.

Go to Create API.

Choose REST API (public)

Endpoint - regional 

Click on create API.

Actions - Create a method. Link lambda to API. Link a lot of stuff.  

Save.

Deploy API. New Stage. deploy. 

Invoke URL. 

Enable Logs for it. ALWAYS. 

Save then.

### Notes

Check Account Billing before enabling any service.










