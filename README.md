# Serverless hello world
This is an example hello world api created with the serverless framework that runs on AWS Lambda. If deployed to AWS an API Gateway gets also created with the specified http path of the Lambda(in the serverless.yml).


## Prerequisites

* You have made you AWS access and secret key available through a provided method, like storing them in the ~/.aws/credentials file or export them into environment variables
* You need to install Node.js  with a minimum version of 6.5.0 
* Then you need to install the serverless CLI with `sudo npm install -g serverless`


## Deploy

* `serverless deploy -v`


## Test

* Now you could invoke the Lambda with `serverless invoke -f hello -l` if everything went fine
* This time we also have an API Gateway which calls the Lambda, so we could curl the API Gateway endpoint to see if everything went fine. You can find the respective URL in the output of `serverless deploy -v`


## Undeploy

* `serverless remove`