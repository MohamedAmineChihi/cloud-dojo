# ArgoCD Infrastructure automation 
---
this 

## Implementation steps:
 
### 1- Using local kubernetes cluster: minikube
### 2- Using cloud configured kubernetes cluster : AKS
### 3- Terraform steps:
`terraform init`
`terraform plan`
`terraform apply`
## Validation steps:
- to check 
`helm list --pending -A`
`helm status argocd -n argocd`