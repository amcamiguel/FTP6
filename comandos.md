**Comandos FTP importantes**

Esta es una lista de los comandos más comunes de utilizar dentro del servidor y una serie de parámetros para modificar estos comandos: ***ls, mkdir, put, get, delete***. Estos cincos comandos son los que vamos a ver, si te interesa saber su funcionamiento en este [enlace](https://docs.oracle.com/cd/E24842_01/html/E22524/remotehowtoaccess-14.html) tienes una breve explicación de como funcionan.

Dos de los parametros que vamos a ver son ***! y m***. La exclamación delante del comando hace que el comando funcione de manera que veamos los archivos del servidor, ya que de manera predeterminada todos los comandos funcionan de manera local, es decir trabajan en el directorio del cliente. Y la m lo que nos permite es que los comandos put, get, delete funcionen de manera masiva, es decir que te permiten la subida, bajada y eliminación de varios archivos a la vez, esto tiene una pega y es que por cada archivo que vamos a "mover" nos preguntará si queremos hacerlo o no, para desactivar esta función podemos usar el comando prompt y así no hará esas preguntas.

*Antes de empezar recordar crear archivos de prueba llamados pruebas.txt tanto en el directorio /home del servidor como el del cliente.*

Después de esta pequeña introducción vamos a pasar con la guía.

El primer comando que veremos es el *ls*, después de conectarnos al servidor si hacemos un ls nos aparecerá lo siguiente:

![imagen1](/imagenes/captura1.png)

Pero si en cambio lo usamos poniendo ! nos aparecerán los directorios del usuario donde estamos alojando el servidor.

![imagen2](/imagenes/captura2.png)

Ahora vamos a probar a crear un directorio en el cliente, al igual que si estuviéramos creando uno en nuestra máquina normal simplemente tendremos que poner mkdir seguido del nombre que queremos que tenga el directorio:

![imagen3](/imagenes/captura3.png)

Si volvemos a hacer un ls podremos comprobar que efectivamente se ha creado el directorio nuevo:

![imagen4](/imagenes/captura4.png)

Obviamente si queremos crearlo en el servidor tendremos que poner la ! delante.

Ahora vamos a ver como subir nuestros archivos desde el cliente al servidor, para ello utilizaremos el comando put, vamos a probar a subir el archivo que hemos creado:

![imagen5](/imagenes/captura5.png)

Y si quisiéramos volver a bajar el archivo en vez de usar el put habría que usar el get:

![imagen6](/imagenes/captura6.png)

Este proceso si hay que pasarlo por cada archivo es un poco engorroso si queremos subir muchos, por eso para subir o bajar muchos archivos tendríamos que usar el parametro *m(mget mput)* y de esta manera si ingresamos mput * nos preguntará que archivos queremos subir.

A continuación vamos a probar a borrar archivos que hayamos subido al servidor:

![imagen7](/imagenes/captura7.png)

Y estas serían las distintas pruebas que vamos a realizar con los comandos.

En este [enlace](FileZilla.md) podrás acceder a la actividad del FileZilla.

[Volver a la página principal](README.md)
