#SWAP-EJERCICIOS DE CLASE TEMA 1

**1. Comparativa de rendimiento y eficiencia entre los servidores web m�s conocidos: Apache, Nginx, Lighttpd, Cherokee y NodeJS.**

***APACHE***
- Gran escalabilidad y robustez, adem�s de f�cilmente configurable.
- Es un sistema multiplataforma y est� disponible para pr�cticamente todos los sistemas operativos, como Microsoft Windows, Linux o Mac.
- En cuanto a rendimiento y capacidad, soporta m�s de 1 mill�n de conexiones.
- Soporta protocolos de seguridad SSL y TL.
- Dada su alta capacidad de configurabilidad y modularidad, permite ampliar f�cilmente tanto sus capacidades como la creaci�n de logs con los que aumentar el control sobre lo que sucede en el servidor.
- Al tratarse de software de c�digo abierto, programadores de todo el mundo contribuyen de forma constante a su mejor�a, lo cual permite a Apache actualizarse constantemente.

***NGINX***
- Software libre de c�digo abierto.
- Soporta servidores virtuales.
- En cuanto a seguridad, soporta SSL.
- Es capaz de habilitar la conexi�n simult�nea de m�s de 10.000 conexiones.
- Est� construido mediante una arquitectura as�ncrona, que deja muy poca huella en la web y consume muy pocos recursos, haci�ndolo ideal para manejar m�ltiples y cambiantes p�ginas web activas.

***LIGHTTPD***
- Software libre, r�pido, seguro y flexible.
- Funciona con m�ltiples plataformas, como Linux, Unix, y en versi�n especial, Lighttpd for Windows, para Microsoft.
- Permite virtual hosting.
- Soporta cifrado SSL en seguridad.
- Admite la instalaci�n de m�dulos externos.
- Es un servidor con arquitectura as�ncrona.
- Puede manejar hasta 10.000 conexiones simult�neas.

***CHEROKEE***
- Posee una velocidad hasta 6 veces m�s r�pido que Apache
- Facilidad de configuraci�n gracias a su panel de control
- Servidor web multiplataforma bajo la licencia GNU
- Se intenta mantener un core reducido �de forma tal que pueda utilizarse en sistemas empotrados- y efectuar todas las funcionalidades como m�dulos cargables en tiempo de ejecuci�n.
- Alta eficiencia y una arquitectura suficientemente flexible para poder escalar a servidores SMP.

***NODEJS***
- A diferencia de Apache que crea un hilo de proceso por cada cliente que pida datos al servidor, Node.js crea solo un hilo de procesos para todos los clientes lo que hace que el servidor soporte muchas m�s conexiones.
- Es OpenSource.
- No hay necesidad de Ajax para poder mantener una conexi�n asincronica con el servidor, gracias a los websockets de html5 y para otros exploradores viejos "IE8-" con polyfills.
- Por lo anterior podemos hacer Chats o aplicaciones web con multiples usuarios de una manera impresionante ejemplos de aplicaciones que usen esto pues, Facebook, Google Plus, Gmail, etc...
- Ya no hay problemas cuando vas a realizar una aplicacion web y tienes que programar en dos lenguajes una para el servidor y otra para el cliente y hacer doble trabajo, con Node.js hay cliente-servidor son  dos gotas de agua totalmente iguales hay transparencia total.

**--> CONCLUSIONES <--**
Nginx es m�s eficiente que Apache a la hora de gestionar un gran n�mero de conexiones concurrentes. Adem�s, consume menos memoria por conexi�n de cliente. Nginx es la alternativa a Apache m�s eficiente que existe.
Nginx y Lighttpd son ideales para los servidores VPS con pocos recursos.
Lighttpd es muy ligero y hace muy poco uso tanto de la RAM como de la CPU.
Cherokee es muy apto para su uso en sistemas empotrados, ya que su n�cleo es muy reducido.
NodeJSn y Cherokee es mejor en cuanto a concurrencia comparado con Apache.
En la actualidad Nginx es el segundo servidor web m�s utilizado, con m�s de un 14% del total de dominios activos.

En definitiva, Apache es el m�s usado, mientras que tanto Ngnix como Lighttpd, al ser as�ncronos, permiten una gran escalabilidad y velocidad.

