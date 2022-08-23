Terranetes with LocalStack example
==================================

Quickly get Terranetes working with LocalStack

Requirements
------------

- docker-compose
- minikube
- helm
- helmfile (optional)

Usage
-----

### tl;dr

```
docker-compose up
minikube start
helmfile sync
kubectl apply -f provider.yaml
kubectl apply -f cfg.yaml
kubectl -n apps annotate configurations bucket "terraform.appvia.io/apply"=true --overwrite
```

### Cleanup

```
kubectl -n apps delete configurations bucket
```
