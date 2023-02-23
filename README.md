## Description

Build a few EC2 instances in AWS using Terraform.

Follow these guidelines when building the AWS resources:
1. do not hard code credentials in code
2. do not store state files in git
3. use modules (eg: use a module for EC2 instance)
4. use AWS S3 remote backend with dynamodb state lock
5. assume terraform role with AWS STS


```

# define AWS creds as env vars
export AWS_ACCESS_KEY_ID=AKIAIOSFODNN7EXAMPLE
export AWS_SECRET_ACCESS_KEY=wJalrXUENG/bPxRfiCYEXAMPLEKEY
export AWS_DEFAULT_REGION=us-west-2

# build resource
terraform plan
terraform apply
```