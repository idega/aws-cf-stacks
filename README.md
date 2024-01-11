# To list stacks
aws cloudformation describe-stacks --region eu-west-1

# To validate template
aws cloudformation validate-template --region eu-west-1 --template-body file://template.yaml

# To create Stack
aws cloudformation create-stack \
    --stack-name TestCloud4ClubIdega \
    --region eu-west-1 \
    --template-body file://template.yaml \
    --parameters file://parameters.json 

# From build directory:
s3cmd put * s3://test.cloud4club.com
