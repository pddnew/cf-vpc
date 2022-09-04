
### Learn AWS CloudFormation
```shell
$ aws --version
aws-cli/2.7.29 Python/3.10.6 Darwin/21.6.0 source/x86_64 prompt/off
```
AWS CLI example:
```shell
$ aws cloudformation create-stack \
  --stack-name myteststack \
  --template-body file:///home/testuser/mytemplate.json \
  --parameters ParameterKey=Parm1,ParameterValue=test1 ParameterKey=Parm2,ParameterValue=test2
```
---
`$ aws cloudformation create-stack --stack-name cf-vpc --template-body file://vpc.yml --parameters ParameterKey=EnvironmentName,ParameterValue=dev`

`$ aws cloudformation list-stack-resources --stack-name cf-vpc`

`$ aws cloudformation update-stack --stack-name cf-vpc --template-body file://vpc.yml --parameters ParameterKey=EnvironmentName,ParameterValue=dev`

`$ aws cloudformation delete-stack --stack-name cf-vpc`

---
[1. User guide: using cli](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-using-cli.html)