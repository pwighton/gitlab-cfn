# Introduction
AWS Cloudformation templates for Gitlab installation on AWS.

### Instructions
```bash
git clone https://gitlab.com/techmaniack/gitlab-cfn.git
cd gitlab-cfn
aws --region us-west-1 cloudformation create-stack --stack-name GitlabStack --template-body file://./gitlab_existing_vpc.template --parameters ParameterKey=KeyName,ParameterValue=<KeyName> ParameterKey=VPC,ParameterValue=<vpc-ID>
```

## Todo
- Add mappings for all regions
- Add parameters for customised installation
- Create cfn template for new vpc installation
