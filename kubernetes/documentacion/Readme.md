# Documentación Docker 

- Versión instalada de docker
```docker --version```

- Ver informacion general
```docker info```
## Imagen
- Descargar una imagen
```docker pull[nombre imagen]```
```docker pull mysql:8.0```

- Ver el listado de imagenes
```docker image ls```

- Eliminar una imagen
```docker rmi [nombre/id de la imagen]```

- Construir una imagen desde un Dockerfile
``` docker build -t [nombre] .```
```docker build .t imagen .```

## Contenedores

- Crear y ejecutar un contenedor
```docker run -d --name [nombre del contenedor] -p[host:contenedor] [nombre de la imagem]```
```docker run -d --name mi_contenedor -p 3307:3306 mysql:8.0```

- Listar contenedores en ejecución
```docker ps```

- Listar todos los contenedores
```docker ps -a```

- Detener un contenedor
```docker stop [nombre/id del contenedor]```
```docker stop mi_contenedor```

- Borrar un contenedor detenido
```docker rm [nombre/id del contenedor]```
```docker rm mi_contenedor```

- EliminR forzando su detenido
```docker rm -f [nombre/id del contenedor]```
```docker rm -f mi_contenedor```

- Iniciar el contenedor
```docker start [nombre/id del contenedor]```

- Reiniciar contenedor
```docker restart [nombre/id del contenedor]```

- Elimina todo sin usar 

# Docker compose
 
- Levantar los servicios definidos en el docker-compose
```docker compose up -d```

- Detener servicios
```docker compose down```