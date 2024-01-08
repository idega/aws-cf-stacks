aws cloudformation describe-stacks --region eu-west-1
aws cloudformation validate-template --region eu-west-1 --template-body file://template.yaml
aws cloudformation create-stack --stack-name TestCloud4Club --region eu-west-1 --template-body file://template.yaml --parameters ParameterKey=ProductDomain,ParameterValue=test.cloud4club.com

