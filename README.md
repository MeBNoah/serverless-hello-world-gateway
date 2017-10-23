# Serverless hello world
This is an example hello world api created with the serverless framework that runs on AWS Lambda. If deployed to AWS an API Gateway with the specified http path of the Lambda, which is specified in the serverless.yml file.


## Prerequisites 

* You have made you AWS access and secret key available through a provided method, like storing them in the ~/.aws/credentials file or export them into environment variables
* You need to install Node.js  with a minimum version of 6.5.0 
* Then you need to install the serverless CLI with `sudo npm install -g serverless` 
* `npm install`


## Deploy 

* `serverless deploy -v`


## Test 

Now you could invoke the Lambda with `serverless invoke -f hello -l` if everything went fine


## Undeploy

* `serverless remove`