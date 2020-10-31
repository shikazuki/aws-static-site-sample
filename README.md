# AWS Static Site Sample

Build Web Static Site on AWS using CloudFormation.
- This WebSite is hosted on AWS S3
- This WebSite is distributed by AWS CloudFront
- This WebSite's access is restricted by OAI

## Use

```
$ aws cloudformation create-stack --stack-name static-site-sample --template-body file://static-site.yaml
```

Then, index.html upload to S3.

```
$ aws s3 cp ./index.html s3://{BucketName(WebStatic)}
```