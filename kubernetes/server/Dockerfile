#instalar nginx
FROM nginx:alpine

#copia el archivo index.html al contenedor
COPY index.html /usr/share/nginx/html/index.html

#expone el puerto 80
EXPOSE 80

#docker build -t nombre . //el . es para la ubicacion
#docker image ls //para ver las imagenes creadas
#docker run -d --name yurben -p 8080:80 yumber //sirve para correr el contenedor en segundo plano y asignarle un nombre y exponer el puerto
#docker ps //para ver los contenedores corriendo