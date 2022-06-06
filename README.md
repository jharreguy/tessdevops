TEST DEVOPS 

En la carpeta diagrama tenemos el test 1: un archivo README.md donde explico todo.

En la carpeta backend y frontend corresponde al test 2

Como se instala, deben primero instalar docker y docker compose

desde una terminal escribimos

git clonehttps://github.com/jharreguy/testdevops.git

Una vez hecho eso dentro de la carpeta backend hacemos

Docker-compose up –d

Por que tiene el archivo docker-compose.yml configurado, esperar que levante la base de datos backend_db pero el backend_web no logre que funcione, le hago una 

Docker run –p 8080:8080 nombre de container

Y me tira error 

Unable to find image '653d462d2654:latest' locally

docker: Error response from daemon: pull access denied for 653d462d2654, repository does not exist or may require 'docker login': denied: requested access to 

the resource is denied.

See 'docker run --help'.

Asi que no lo pude hacer funcionar, en el archivo settings se debe poner el usuario, clave y bases de datos, que debe coincidir con el docker-compose.yml

ademas debemos poner una SECRET KEY pero yo no super como configurarlo por que no debe ir vacio.

con respecto al frontend, debemos ingresar a dicha carpeta y alli tenemos el archivo docker-compose.yml

el ejercicio solicitaba que frontend y backend esten en el mismo docker compose pero no lo hice asi

entonces hacemos docker-compose up -d

y nos levanta a aplicacion localhost:3000, pero no va a funcionar por que no falta el backend web

En la carpeta nginx corresponde al test 3 


