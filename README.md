# RootCheck CloudFormation



## Prep Lambda Code

1. Create a ZIP file of the source code files in RootActivityLambda.  The files should be in the root of the zip file.

2. Upload the file to your favorite S3 bucket



## How To Setup a CodePipeline

Create a stack using 'RootAPIMonitor.yaml' using below input values

Input Parameter Values

- CloudWatchLogDestinationArn:

  ARN of Cloudwatch Log in remote account where Cloudwatch log subscription will send log info.

- CloudWatchLogGroupName:

  Name of a local Cloudwatch Log Group where this trigger sends alert messages

- LambdaTimeout

  Enter a timeout value in seconds for the lambda function. Min is 3, max is 300 and default is 60.

- LambdaS3Bucket:

  Name of the S3 bucket where the lambda function is stored

- LambdaS3Key:

  Name of the S3 key of the Lambda function (include the prefix as well)







