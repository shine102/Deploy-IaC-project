# Deploy-IaC-project

## Pre-requisites

- Create an S3 bucket contain code file "source.zip".
- Replace the bucket name in the "server-parameters" file.
- Adjust the "server-parameters" file to your needs.

## Deploy
```bash
aws cloudformation create-stack --stack-name $stackname --template-body file://final-project.yml --parameters file://server-parameters --capabilities CAPABILITY_NAMED_IAM --region $region --profile $profile 
```

