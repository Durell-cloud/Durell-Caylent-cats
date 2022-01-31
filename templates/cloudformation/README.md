# Cloudformation-project
1. Stack Names: Network-stack,Compute-stack

2. Resource Template Name : Network_stack.yml , Compute_stack.yml

3. Lucid charts AWS Project Diagram: Architecture.png




# CLI commands:
-----------------

#create network stack first and validate in cloudformation whether teh stack is succefully created or not(Wait atleast 10 mins)


aws cloudformation create-stack --stack-name Network-stack  --template-body file://Network_stack.yml --region=us-east-1 --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM

#create compute stack once network stack is completed


aws cloudformation create-stack --stack-name Compute-stack  --template-body file://Compute_stack.yml --region=us-east-1 --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM





