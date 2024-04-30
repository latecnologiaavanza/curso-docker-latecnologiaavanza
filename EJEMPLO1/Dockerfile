#Indicamos la imagen que vamos a utilizar
FROM ubuntu:latest

#Instalamos algunas heramientas
RUN apt-get update && apt-get install -y curl wget vim git

WORKDIR /app

#Creamos un archivo de texto dentro del contenedor
RUN echo "¡Hola Docker!" > saludo.txt

EXPOSE 80

CMD ["echo","Este es un contenedor de ejemplo"]