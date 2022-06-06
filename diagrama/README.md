los usuarios son redirigidos en el balanceador de carga entre la instancia "A" y la instancia "B", ademas cada uno tiene si auto scalling programado, ambos 

servidores con frontend JS y como backend en la instancia "A" una base de datos no relacional y en la instancia "B" una relacional

DIFERENCIAS SQL Y NOSQL


Bases de Datos relacionales

Las bases de datos relacionales se caracterizan por ser una colección ordenada de registros que se organizan en un conjunto de tablas. Estas tablas se relacionan entre sí, dando lugar a una base de datos desde donde se puede acceder a los datos o volver a montarlos de muchas maneras diferentes sin tener que reorganizar las tablas de la base.

Para acceder a estos datos, usaremos lo que se conoce como Lenguaje de Consultas Estructuradas, (SQL, Structured Query Language). Con SQL podemos obtener y alterar datos de una forma organizada siempre y cuando tengamos en cuenta cuál es la estructura de la base de datos con la que estamos trabajando. Para ello, utilizaremos los distintos comandos que SQL pone a nuestra disposición.

Las bases de datos relacionales se organizan a través de identificadores. De este modo, cada tabla tiene un identificador único que es el que va a establecer su relación con el resto de tablas. A su vez, estos identificadores hacen que sea más fácil organizar cada una de las tablas por separado.

En cuanto a los formatos que se utilizan en este tipo de bases de datos, suele ser el formato tabla, (Un ejemplo serían las hojas de Excel o Access) y los registros se organizarían por filas y columnas.

Los principales sistemas gestores de bases de datos relacionales son: MySQL, MariaDB, SQLite, PostgreSQL, SQL Server y Oracle.

Bases de datos no relacionales

Las bases de datos no relacionales están diseñadas para modelos de datos específicos y que no necesitan ser relacionados con otros modelos. Cada tabla funciona de forma independiente y son mucho más sencillas que los modelos relacionales.

Esta sencillez de acceso y de ordenación de la base de datos hace que en el panorama actual estén cobrando más importancia que las relacionales.

Las bases de datos no relacionales pueden tener identificador único, es decir, para identificar cada uno de los registros de la base de datos, pero este identificador no se usará (generalmente) para relacionar unos registros con otros. Como veremos, la información se organiza normalmente mediante documentos y es muy útil cuando no tenemos un esquema exacto de lo que se va a almacenar.

Con respecto a los formatos que se utilizan en las bases de datos no relacionales, podríamos decir que el formato más popular es el del documento. En muchos casos, lo que se utiliza es un objeto con una clave y un valor para que el acceso a la información sea pueda realizar de una forma sencilla.

Los principales sistemas gestores de bases de datos no relacionales son: MongoDB, Redis y Cassandra

fuente:https://codenotch.com/blog/diferencias-entre-bases-de-datos-relacionales-y-no-relacionales/
