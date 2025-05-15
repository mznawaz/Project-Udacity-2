# Project-Udacity-2

Script - 1
aws cloudformation create-stack \
  --stack-name udagram-networking \
  --template-body file://networking.yaml \
  --parameters file://initial-params-for-networkingyaml.json \
  --capabilities CAPABILITY_NAMED_IAM
  
Script 2 - 
aws cloudformation create-stack \
  --stack-name udagram-app \
  --template-body file://application.yml \
  --parameters file://params.json \
  --capabilities CAPABILITY_NAMED_IAM

Script 3 - To delete the CFN template
aws cloudformation delete-stack --stack-name udagram-networking --region us-east-1
aws cloudformation delete-stack --stack-name udagram-app --region us-east-1

Load balancer URL - 
UdagramALB-1187042844.us-east-1.elb.amazonaws.com
