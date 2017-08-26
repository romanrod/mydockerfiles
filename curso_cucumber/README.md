WIP
Crear el container a partir del Dockerfile. Posicionado donde se encuentra el archivo Dockerfile, ejecutar la siguiente instrucción:

$ docker build t- curso_cucumber .

Para levantar el container y nos quede una terminal lista para trabajar, primero habrá que crear una carpeta donde se encuentre el archivo Dockerfile, podríamos llamarla proyectoy hay que colocar la ruta completa de la ubicacin de dicha carpeta

Windows:
Para conocer la ruta actual en la consola de comandos, escribir la siguiente linea y copiar el resultado que devuelve:

   echo %cd%

Esa será la carpeta donde se está posicionado que es la misma carpeta donde está el Dockerfile.

$ docker run -v <la ruta completa>/proyecto:/proyecto --add-host="localhost:<ip>" -ti curso_cucumber bash

Pending: Obtener el valor de ip
