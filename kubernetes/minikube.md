# Hands on minikube

## Minikube

I. Start

develop

```
minikube start --profile=develop --cpus=4 --memory=4096 --driver=docker
```

II. Profile list

```
minikube profile list
```

III. Use profile

```
minikube profile develop
```

IV. K8S Nodos
```
kubectl get nodes
```

IV. K8S Context
```
kubectl config current-context
```




II. Profile

```
eval $(minikube -p <nombre-del-perfil> docker-env)
```

Note:
Minikube error build for buildkit.
```
export COMPOSE_DOCKER_CLI_BUILD=0
export DOCKER_BUILDKIT=0
```

III. Enable docker

```
eval $(minikube docker-env)
```


V. List image

```
minikube image ls --format table
```