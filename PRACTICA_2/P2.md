##PRÁCTICA 2 - Clonar la información de un sitio web

**2. Crear un tar con ficheros locales en un equipo remoto.**

*tar czf - /home/mariamma | ssh 192.168.111.137 'cat > ~/tar.tgz'*

Con este comando copiamos el directorio **mariamma** en nuestra máquina2 cuya IP es 192.168.111.137

![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/1.PNG  "Ejecución del comando en la maquina1")
![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/2.PNG  "Comprobación en la máquina2")



**3. Instalar la herramienta rync.**

Para ello utilizamos el comando: *sudo apt-get install rsync*

![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/3.PNG  "Instalacion rsync máquina1")
![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/4.PNG  "Instalacion rsync máquina2")

Para probar el funcionamiento de rsync, clonamos una carpeta cualquiera, en este caso clonamos la carpeta 
que posee el contenido del servidor web principal.

*rsync -avz -e ssg root@ubuntu1:/var/www/ /var/www/*

![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/5.PNG  "Estado de apache en la máquina1")

Y seguidamente comprobamos que ambas máquinas poseen lo mismo en el directorio **/var/www**

![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/6.PNG  "Contenido /var/www maquina1")
![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/7.PNG  "Contenido /var/www maquina2")


**4. Acceso sin contraseña para ssh.**

Generamos la clave en la máquina secundaria: **ssh-keygen -t dsa**

![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/8.PNG  "Generacion de clave")

Seguidamente copiamos la clave generada en el archivo authorized_keys tal y como muestra la siguiente imagen.

![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/9.PNG  "Clave generada")

Y por último se hace la copia de la clave a la máquina principal(que es a la cual queremos acceder luego desde la máquina secundaria)

![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/10.PNG  "Copia de clave")

Ahora podremos conectarnos desde la máquina dos a la uno de forma remota:
![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/11.PNG  "Acceso remoto a la máquina1")


**5. Porgramas tareas con contrab.**

En este caso programamos el crontab para que todos los lunes a las 06:30 se actualicen todos los cambios realizados en **/var/www** existente
en la maquina1 a la máquina2.

![img](https://github.com/MariaMma6/SWAP/blob/master/imagenes/imgP2/12.PNG  "Crontab modificado")
