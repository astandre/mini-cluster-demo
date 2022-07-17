# Applications

# Run app1
Build 
```shell
  docker build -t app1 -f ./apps/app1/Dockerfile  .
```

Listar imagenes
```shell
  docker image ls	
```

Listar contenedores
```shell
docker container ls	
```

Ejecutar contenedores
```shell
   docker run -d -p 3000:3000 app1 
```

Conectarse a istancia
```shell
   docker exec -it  friendly_hofstadter bash
```



