After adding provider in main.tf file run the following command

- terraform init

to apply the changes run the following command

- terraform apply

to destroy all resource run:

- terraform destroy

CDK Bootstrap Command:
aws cloudformation create-stack --stack-name CDKToolkit --template-body file://cdk-bootstrap-stack.yaml --parameters file://config/cdk-bootstrap-stack-params.json --region ap-south-1 --capabilities "CAPABILITY_NAMED_IAM" "CAPABILITY_AUTO_EXPAND"

aws cloudformation update-stack --stack-name CDKToolkit --template-body file://cdk-bootstrap-stack.yaml --parameters file://config/cdk-bootstrap-stack-params.json --region ap-south-1 --capabilities "CAPABILITY_NAMED_IAM" "CAPABILITY_AUTO_EXPAND"

aws cloudformation delete-stack --stack-name CDKToolkit --region ap-south-1
