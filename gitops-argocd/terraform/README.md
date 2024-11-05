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

### After deploying ArgoCD on K8s cluster
- Check pods:
`kubectl get pods -n argocd `

- Check secrets:

`kubectl get secrets argocd-initial-admin-secret -o yaml -n argocd` 

- convert password to base 64:
`echo <password> | base64 -d`
- to access ArgoCD:
`kubectl port-forward svc/argocd-server -n argocd 8080:80`