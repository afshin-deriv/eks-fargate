# eks-fargate

export AWS_SECRET_ACCESS_KEY="XXXXXX"

export AWS_ACCESS_KEY_ID="XXXXXX"


terraform apply -auto-approve -var-file=production.tfvars

aws eks describe-cluster --name eks_cluster-default

kubectl apply -f configmap.yaml