

- Create pod:
`microk8s kubectl apply -f fastapi-pod.yaml`

- Create service:
`microk8s kubectl apply -f fastapi-service.yaml`

- Port forwarding for local access:

`microk8s kubectl port-forward pod/fastapi-api 8080:8000`