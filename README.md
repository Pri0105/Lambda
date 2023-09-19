# Lambda
Lambda for Cost Optimization:

1. Create a Lambda Function which will be triggered by CloudWatch daily or weekly basis
2. The Lambda function with the help of Python boto3 module will check for the snapshots which are not attached to any volume or a volume that is not attached to an EC2 instance,will delete the snapshot and the volume if not attached to an EC2 instance.

3. It will also check the last used date of the snapshot, if more than 30 days, it will delete the snapshot.
