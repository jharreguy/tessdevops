TEST DEVOPS 

En la carpeta diagrama tenemos el test 1

En la carpeta backend y frontend corresponde al test 2

Como se instala, deben primero instalar docker y docker compose

Una vez hecho eso dentro de la carpeta backend hacemos

Docker-compose up –d

Por que tiene el archivo docker-compose.yml configurado, esperar que levante la base de datos backend_db pero el backend_web no logre que funcione, le hago una 

Docker run –p 8080:8080 nombre de container

Y me tira error 

Unable to find image '653d462d2654:latest' locally

docker: Error response from daemon: pull access denied for 653d462d2654, repository does not exist or may require 'docker login': denied: requested access to 

the resource is denied.

See 'docker run --help'.

Asi que no lo pude hacer funcionar, en el archivo settings.

En la carpeta nginx corresponde al test 3 
