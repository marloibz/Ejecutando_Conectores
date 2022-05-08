# Ejecutando_Conectores
explicaré lo que sucede en los ejemplos 1, 2 y 4 de los apuntes de Docker para desarrolladores.


# Ejemplo 1
Para empezar descargaremos una imagen previa usamos el comando docker pull ubuntu:18.04 y veríamos algo así:
![1](https://user-images.githubusercontent.com/91874499/167297510-c0898a46-a5fd-461f-be4f-23c30c798398.PNG)

Ahora vamos a crear un contenedor de ubuntu:18.04 para tener acceso a un shell en él con el comando :docker run -it ubuntu:18.04 /bin/bash

root@ef2bea1d6cb1:/#
![2](https://user-images.githubusercontent.com/91874499/167297576-79a3a314-c7e7-4394-ac7e-10dff10a1be2.PNG)

Y como vemos hacemos una comprovacion de que todo ha ido correctamente.


# Ejemplo 2

Para crear un contenedor de centOS:18.04 y listar el contenido de la carpeta /.Con el comando : docker run ubuntu:18.04 ls/. Y para comprobar que todo ha ido bien nos tendría que mostrar lo siguiente en la consola

![3](https://user-images.githubusercontent.com/91874499/167297719-4e909a3c-9c54-49b3-81bd-c44b49026972.PNG)

# Ejemplo 4

Lo primero es crear un contenedor de debian 9 y lo haremos con el comando: docker run it -it -w /etc debian:9 ls

![4](https://user-images.githubusercontent.com/91874499/167297793-e9feafc6-24e6-4f2b-a88b-cb59bb739b30.PNG)

Lo siguiente será mostrar los contenedores en ejecución con el comando: docker ps

![5](https://user-images.githubusercontent.com/91874499/167297850-4e1f6309-0c41-40a0-8e00-feb6df000906.PNG)

Ahora mostraremos todos los contenedores creados ya estén en ejecución (Estado Up) o parados (Estado Exited) con el comando : docker ps -a


![6](https://user-images.githubusercontent.com/91874499/167297909-aa2df663-3db0-4816-a2fb-ab00b00326b4.PNG)


