**Comandos FTP importantes**

Esta es una lista de los comandos más comunes de utilizar dentro del servidor y una serie de parámetros para modificar estos comandos: ***ls, mkdir, put, get, delete***. Estos cincos comandos son los que vamos a ver, si te interesa saber su funcionamiento en este [enlace](https://docs.oracle.com/cd/E24842_01/html/E22524/remotehowtoaccess-14.html) tienes una breve explicación de como funcionan.

Dos de los parametros que vamos a ver son ***! y m***. La exclamación delante del comando hace que el comando funcione de manera que veamos los archivos del servidor, ya que de manera predeterminada todos los comandos funcionan de manera local, es decir trabajan en el directorio del cliente. Y la m lo que nos permite es que los comandos put, get, delete funcionen de manera masiva, es decir que te permiten la subida, bajada y eliminación de varios archivos a la vez, esto tiene una pega y es que por cada archivo que vamos a "mover" nos preguntará si queremos hacerlo o no, para desactivar esta función podemos usar el comando prompt y así no hará esas preguntas.

*Antes de empezar recordar crear archivos de prueba llamados pruebas.txt tanto en el directorio /home del servidor como el del cliente.*

Después de esta pequeña introducción vamos a pasar con la guía.

El primer comando que veremos es el *ls*, después de conectarnos al servidor si hacemos un ls nos aparecerá lo siguiente:
![imagen1](/Imagenes/captura1.png)
