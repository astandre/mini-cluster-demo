# Applications

## Build

```shell
  docker build -t app1 -f ./apps/app1/Dockerfile  .
```

## Listar imagenes

```shell
  docker image ls	
```


## Tagear imagen

```shell
  docker tag astandre/app1 astandre/app1:latest
```

## Publicar imagen

```shell
  docker push astandre/app1:latest
```

## Listar contenedores

```shell
docker container ls	
```

## Ejecutar contenedores

```shell
   docker run -d -p 3000:3000 app1 
```

## Conectarse a istancia

```shell
   docker exec -it  friendly_hofstadter bash
```

## Docker compose

```shell
   docker-compose up -d
```



# Cluster


## Start cluster

```shell
minikube start
```



## Generar compose

```shell
kompose convert --out cluster.yaml
```

## Run cluster

```shell
kubectl apply -f cluster.yaml
```

## Abrir servicios

```shell
minikube service --all
```

## Ver pods

```shell
kubectl get pods
```

## Describir pods

```shell
kubectl describe pods
```

## Ver servicios

```shell
kubectl get services
```

## Dashboard

```shell
minikube dashboard
```
