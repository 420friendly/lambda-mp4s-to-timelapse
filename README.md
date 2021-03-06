# lambda-mp4s-to-timelapse

converts a slew of mp4s from s3 into a timelapse with music

# Usage

Invoke this function like any lambda function, as documented in the aws sdk.

- [JavaScript](http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/Lambda.html#invoke-property)
- [Ruby](http://docs.aws.amazon.com/sdkforruby/api/Aws/Lambda/Client.html#invoke-instance_method)
- [PHP](http://docs.aws.amazon.com/aws-sdk-php/latest/class-Aws.Lambda.LambdaClient.html#_invokeAsync)
- [Python](http://boto.readthedocs.org/en/latest/)
- OR on the function's "edit" tab via amazon's interface
- OR via the AWS CLI

# Payload

## required

- `sourceBucket` - S3 bucket for the mp4s to be used
- `sourceDir` - S3 keys prefix (folder) for the mp4s
- `musicUrl` - Url for an mp3 to be downloaded and included in the timelapse
- `destBucket` - S3 bucket to dump the timelapse into
- `destKey` - Key for the file to be saved to on S3

