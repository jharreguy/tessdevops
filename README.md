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

para utilizar tener un proxy de nginx lo unico que tenemos que es ni bien descargamos los archivos con git clone, ingresamos a la carpeta NGINX y corremos 

el docker-compose up -d

y alli vamos a tener la posibilidad que en un solo servidor, poder tener varios sitios web, en cada sitio apuntamos a la misma ip ejemplo compramos dos 

dominios en namecheap entonces le ponemos la misma ip y dns, luego en el hosting le asignamos la ip publica, y el proxy de nginx se encarga de redirigir a 

que sitio corresponde segun lo que haya tipieado el usuario, ademas la ventaja que tiene es que instala un certificado SSL gratis, y por ultimo si 

modificamos el index.html impacta la modificacion en el sitio al momento.



