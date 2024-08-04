# Starter

This starter repository provides scripts to serve services I usually need for my projects such as containers for databases and local mail storage.

All of the scripts are executable as a `make` command:

1. `make postgres-up` : start postgresql database in a docker container
2. `make postgres-down` : stop the currently active postgresql container
3. `make mongo-up` : start mongo database in a docker container
4. `make mongo-down` : stop the currently active mongodb container
5. `make mailhog-up` : start mailhog in a docker container
6. `make mailhog-down` : stop the currently active mailhog container

## Deploying to Docker Compose

To deploy to compose, run:

```
docker-compose -f docker/docker-compose.yaml up -d
```

## Deploying to Kubernetes

To deploy to kubernetes locally, run:

```
kubectl apply -f ./kubernetes
```
