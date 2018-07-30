A sample project to demonstrate streaming Lambda and API Gateway Cloudwatch logs to S3 via Kinesis Firehose.

https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs//SubscriptionFilters.html#FirehoseExample

### Deploy:

`yarn sls deploy --stage dev`

### IAM Notes:

API Gateway must have a role configured allowing it to push logs to Cloudwatch.  If this role does not exist, a log group will not be created, and the stack deployment will fail.