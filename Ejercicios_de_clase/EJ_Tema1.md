#SWAP-EJERCICIOS DE CLASE TEMA 1

**1. Comparativa de rendimiento y eficiencia entre los servidores web más conocidos: Apache, Nginx, Lighttpd, Cherokee y NodeJS.**

***APACHE***
- Gran escalabilidad y robustez, además de fácilmente configurable.
- Es un sistema multiplataforma y está disponible para prácticamente todos los sistemas operativos, como Microsoft Windows, Linux o Mac.
- En cuanto a rendimiento y capacidad, soporta más de 1 millón de conexiones.
- Soporta protocolos de seguridad SSL y TL.
- Dada su alta capacidad de configurabilidad y modularidad, permite ampliar fácilmente tanto sus capacidades como la creación de logs con los que aumentar el control sobre lo que sucede en el servidor.
- Al tratarse de software de código abierto, programadores de todo el mundo contribuyen de forma constante a su mejoría, lo cual permite a Apache actualizarse constantemente.

***NGINX***
- Software libre de código abierto.
- Soporta servidores virtuales.
- En cuanto a seguridad, soporta SSL.
- Es capaz de habilitar la conexión simultánea de más de 10.000 conexiones.
- Está construido mediante una arquitectura asíncrona, que deja muy poca huella en la web y consume muy pocos recursos, haciéndolo ideal para manejar múltiples y cambiantes páginas web activas.

***LIGHTTPD***
- Software libre, rápido, seguro y flexible.
- Funciona con múltiples plataformas, como Linux, Unix, y en versión especial, Lighttpd for Windows, para Microsoft.
- Permite virtual hosting.
- Soporta cifrado SSL en seguridad.
- Admite la instalación de módulos externos.
- Es un servidor con arquitectura asíncrona.
- Puede manejar hasta 10.000 conexiones simultáneas.

***CHEROKEE***
- Posee una velocidad hasta 6 veces más rápido que Apache
- Facilidad de configuración gracias a su panel de control
- Servidor web multiplataforma bajo la licencia GNU
- Se intenta mantener un core reducido –de forma tal que pueda utilizarse en sistemas empotrados- y efectuar todas las funcionalidades como módulos cargables en tiempo de ejecución.
- Alta eficiencia y una arquitectura suficientemente flexible para poder escalar a servidores SMP.

***NODEJS***
- A diferencia de Apache que crea un hilo de proceso por cada cliente que pida datos al servidor, Node.js crea solo un hilo de procesos para todos los clientes lo que hace que el servidor soporte muchas más conexiones.
- Es OpenSource.
- No hay necesidad de Ajax para poder mantener una conexión asincronica con el servidor, gracias a los websockets de html5 y para otros exploradores viejos "IE8-" con polyfills.
- Por lo anterior podemos hacer Chats o aplicaciones web con multiples usuarios de una manera impresionante ejemplos de aplicaciones que usen esto pues, Facebook, Google Plus, Gmail, etc...
- Ya no hay problemas cuando vas a realizar una aplicacion web y tienes que programar en dos lenguajes una para el servidor y otra para el cliente y hacer doble trabajo, con Node.js hay cliente-servidor son  dos gotas de agua totalmente iguales hay transparencia total.

**--> CONCLUSIONES <--**
Nginx es más eficiente que Apache a la hora de gestionar un gran número de conexiones concurrentes. Además, consume menos memoria por conexión de cliente. Nginx es la alternativa a Apache más eficiente que existe.
Nginx y Lighttpd son ideales para los servidores VPS con pocos recursos.
Lighttpd es muy ligero y hace muy poco uso tanto de la RAM como de la CPU.
Cherokee es muy apto para su uso en sistemas empotrados, ya que su núcleo es muy reducido.
NodeJSn y Cherokee es mejor en cuanto a concurrencia comparado con Apache.
En la actualidad Nginx es el segundo servidor web más utilizado, con más de un 14% del total de dominios activos.

En definitiva, Apache es el más usado, mientras que tanto Ngnix como Lighttpd, al ser asíncronos, permiten una gran escalabilidad y velocidad.

