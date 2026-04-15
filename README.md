Terraform EKS Infra Setup
After EKS Cluster is successfully created use the following command to update kube config file to run kubectl commands:
aws eks update-kubeconfig --region $(terraform output -raw region) --name $(terraform output -raw cluster_name)