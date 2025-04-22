🚀 **Guía completa y práctica de comandos Docker por categorías**


## 🧱 1. Imágenes (Images)

| Comando                                 | Descripción                                        |
|-----------------------------------------|----------------------------------------------------|
| `docker build -t nombre .`              | Construye una imagen desde un Dockerfile.         |
| `docker images`                         | Lista todas las imágenes locales.                 |
| `docker rmi nombre`                     | Elimina una imagen.                               |
| `docker tag img nuevo-nombre`          | Renombra/etiqueta una imagen.                     |
| `docker pull nombre`                    | Descarga una imagen desde Docker Hub.             |
| `docker push nombre`                    | Sube una imagen a Docker Hub. (Requiere login)    |


## 📦 2. Contenedores (Containers)

| Comando                                       | Descripción                                               |
|-----------------------------------------------|-----------------------------------------------------------|
| `docker run imagen`                           | Corre una imagen.                                         |
| `docker run -it imagen`                       | Ejecuta en modo interactivo.                              |
| `docker run -d imagen`                        | Ejecuta en segundo plano (detached).                      |
| `docker run --name miapp imagen`              | Le pone nombre al contenedor.                             |
| `docker run -p 8080:80 imagen`                | Mapea puertos host:contenedor.                            |
| `docker ps`                                   | Muestra contenedores activos.                             |
| `docker ps -a`                                | Muestra todos los contenedores (incluidos parados).       |
| `docker start nombre`                         | Inicia un contenedor parado.                              |
| `docker stop nombre`                          | Detiene un contenedor.                                    |
| `docker restart nombre`                       | Reinicia un contenedor.                                   |
| `docker rm nombre`                            | Elimina un contenedor.                                    |
| `docker exec -it nombre bash`                 | Entra a un contenedor corriendo.                          |
| `docker logs nombre`                          | Muestra logs del contenedor.                              |


## ⚙️ 3. Volúmenes y Persistencia

| Comando                                      | Descripción                                    |
|----------------------------------------------|------------------------------------------------|
| `docker volume create nombre`               | Crea un volumen persistente.                  |
| `docker volume ls`                          | Lista todos los volúmenes.                    |
| `docker volume rm nombre`                   | Elimina un volumen.                           |
| `docker run -v nombre:/ruta imagen`         | Monta un volumen en un contenedor.            |


## 🕸️ 4. Redes

| Comando                                           | Descripción                                  |
|---------------------------------------------------|----------------------------------------------|
| `docker network ls`                               | Lista las redes Docker.                      |
| `docker network create nombre`                    | Crea una red.                                |
| `docker network connect red contenedor`           | Conecta un contenedor a una red.             |
| `docker network inspect nombre`                   | Muestra detalles de una red.                 |


## 📄 5. Docker Compose

| Comando                      | Descripción                                       |
|------------------------------|---------------------------------------------------|
| `docker compose up`          | Levanta todos los servicios definidos.           |
| `docker compose up -d`       | Lo mismo pero en segundo plano.                  |
| `docker compose down`        | Detiene y elimina los servicios.                 |
| `docker compose build`       | Construye las imágenes definidas.                |


## 🔍 6. Utilidades

| Comando                      | Descripción                                                |
|------------------------------|------------------------------------------------------------|
| `docker inspect nombre`      | Devuelve info detallada en JSON.                          |
| `docker system df`           | Muestra cuánto espacio ocupan imágenes/contenedores.      |
| `docker system prune`        | Limpia recursos sin usar (¡cuidado!).                     |


## 🧪 7. Avanzado

| Comando                          | Descripción                                     |
|----------------------------------|-------------------------------------------------|
| `docker save` / `docker load`    | Exporta/importa una imagen como `.tar`.        |
| `docker export` / `docker import`| Exporta/importa un contenedor.                 |
