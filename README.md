# Practica 4 - Despliegue con Docker Compose

Este repositorio contiene la configuracion de Docker Compose para desplegar la aplicacion completa (MongoDB, backend y frontend) usando contenedores.

## Repositorios relacionados

- Backend: https://github.com/sergiocruz2004/App_Pr-ctica_2
- Frontend: https://github.com/sergiocruz2004/Frontend_Practica_4

## Requisitos previos

- Docker
- Docker Compose

## Instalacion y ejecucion

1. Clona este repositorio y los otros dos como carpetas hermanas:

git clone https://github.com/sergiocruz2004/Practica4_Docker_Compose.git Proyecto
cd Proyecto
git clone https://github.com/sergiocruz2004/App_Pr-ctica_2.git APPSC
git clone https://github.com/sergiocruz2004/Frontend_Practica_4.git FAPPSC

2. Levanta los tres servicios:

docker-compose up --build -d

3. Verifica que los tres contenedores esten corriendo:

docker ps

## Acceso a los servicios

- Frontend: http://IP_DE_LA_MAQUINA:5173
- Backend (API): http://IP_DE_LA_MAQUINA:3000/api
- MongoDB: puerto 27017 (usuario: admin, contrasena: password123)

## Detener los servicios

docker-compose down
