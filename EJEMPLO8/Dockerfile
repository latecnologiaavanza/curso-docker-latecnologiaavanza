#Stage 1 - Le asignamos un nombre a esta etapa
FROM node:alpine AS build

WORKDIR /app

COPY app /app

#Stage 2 - Inciamos una nueva etapa en la imagen nginx
FROM nginx:alpine AS final

COPY --from=build /app /usr/share/nginx/html

EXPOSE 80

CMD [ "nginx","-g","daemon off;"]