# docker1
# docker_demos
hola mundo con docker

# ubuntu 
imagen:tag

# docker -v
revisa el funcionamiento de docker
# docker images
muestra las imagenes 
# docker ps
muestra los contenedores activos
# docker ps -a
muestra los contenedores apagados
# docker -u
version de docker
# docker pull ubuntu:latest
descarga la imagen de ubuntu
# docker rmi id_imagen
borra una imagen
# docker run
ejecuta la imagen(si no esta instalada se descarga)
# docker run -it ubuntu:18.04
corriendo contenedores dentro de contenedores
# apt update
# apt install python3

# docker start -i c3de9e8faea9

# apt update
actualizar dependencias
# apt install python3
instala python
# docker inspect bd98ece8614d
inspecciona todos los datos del contenedor
# docker commit bd98ece8614d
control de versiones, subir commit
# docker commit bd98ece8614d web_server:latest
commit con nombre
# docker image prune
borra lo pendiente
# docker run --name servidor1 web_server:latest
crear un nuevo contenedor, colocandole nombre y va a estar basado en la imagen web_server:latest
# docker rm id_contenedor
borrar contenedor
# docker save web_server:latest > web_server:latest.tar.
decarga la imagen y la comprime
# docker load -i web_server:latest.tar
es para cargar el archivo descargado
# docker build .
el punto indica donde debe buscar
# docker build -t mi_aplicacion:latest .
darle nombre a la imagen