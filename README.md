# Servidores-Linux-Ubuntu-Readme-DM

Apuntes de Configuracion de **Servidor en Linux**, todos las distribuciones probadas, Ububtu server.

- Autor: Alexander Jair Rojas Paria
--------------

# 📱 Servidores Linux


## Roles de un Administrador


#### Habilidades clave:



* Control de accesos.
* Monitoreo del sistema.
* Administración de recursos.
* Troubleshooting.
* Instalación y mantenimiento de software.
* Creación de respaldos.
* Documentación.
* 


#### **Roles que puedes desempeñar:**



* DevOps Engineer:
    * Se enfocan en los procesos y metodologías para la correcta liberación en el proceso de desarrollo de software.
* Site Reliability Engineer:
    * Se enfocan en que los sistemas de software operen de manera correcta y con el mayor grado de confiabilidad posible.
* Security Operations Engineer:
    * Encargados de mantener la seguridad de los sistemas a nivel de red y aplicaciones.
* Algunos otros roles:
    * Network Engineer.
    * Database Administrator.
    * Network Operation Center Engineer.
    * MLOps Engineer.
    * Cloud Engineer.


## **Servidores?**

Son computadoras especializadas que almacenan y distribuyen información y servicios a otras computadoras en una red. Se utilizan para alojar sitios web, correo electrónico, aplicaciones, bases de datos, juegos en línea, entre otros. \
Además, también pueden ser utilizados para procesar información y realizar tareas complejas que requieren mucha potencia de procesamiento.


## **Sistema Linux/UNIX**

_OS (Sistema Operativo) = Windows, MacOS, GNU/Linux -> GNU/Linux = Linux (Kernel) + GNU (GNU’s Not Unix") -> Linux = Distribuciones_


#### **Distribuciones para Servidores**



* CentOS: Derivada del código fuente de Red Hat Enterprise Linux (RHEL). Es muy estable y está diseñada para ser utilizada en entornos empresariales y de servidores.
* Ubuntu Server: es una versión de Ubuntu diseñada específicamente para su uso en servidores. Ofrece una combinación de facilidad de uso y estabilidad.
* Debian: es una distribución de GNU/Linux muy estable y confiable que es muy popular entre los administradores de sistemas.
* Fedora Server: Impulsada por la comunidad que se enfoca en la innovación y la adopción temprana de nuevas tecnologías.
* Arch Linux: es una distribución muy personalizable y dirigida a usuarios avanzados. Es muy popular entre los administradores de sistemas que prefieren una configuración a medida.
* 


## **Arquitectura de un Sistema**

Es a la estructura y organización interna del sistema operativo. Diseñada para proporcionar una base sólida y segura para la ejecución de aplicaciones y procesos.


#### **Componentes principales**



* Hardware \
Son todos los dispositivos físicos conectados al sistema (discos, mouse, memoria, procesador, teclado, etc.).
* Kernel \
Es una pieza de software que nos permite controlar todo el hardware de nuestro servidor, como el uso de CPU o memoria RAM.
* Shell \
Es la interfaz que está entre el kernel y el usuario. Es quien nos permite ejecutar comandos y pasarlos a un sistema de bajo nivel.
* Aplicaciones \
Es donde el usuario directamente interactúa. Es la capa donde trabajan nuestros comandos y aplicaciones.


## **Diferencias entre: Software Libre y Open Source**


<table>
  <tr>
   <td>Característica
   </td>
   <td>Software Libre
   </td>
   <td>Open Source
   </td>
  </tr>
  <tr>
   <td>Definición
   </td>
   <td>El software otorga al usuario final la libertad de usar, estudiar, copiar, modificar y distribuir el software y sus fuentes
   </td>
   <td>El software cuyo código fuente está disponible públicamente y puede ser examinado, modificado y distribuido por cualquier persona
   </td>
  </tr>
  <tr>
   <td>Filosofía
   </td>
   <td>Se basa en el valor de la libertad del usuario y la creencia de que el conocimiento y la información deben ser libres
   </td>
   <td>Se centra en la colaboración y la revisión del código fuente para mejorar y hacer avanzar el software
   </td>
  </tr>
  <tr>
   <td>Licencias
   </td>
   <td>Utiliza licencias GPL, LGPL, BSD, MIT, Apache, entre otras
   </td>
   <td>Utiliza licencias como la Apache, BSD, MIT, entre otras
   </td>
  </tr>
  <tr>
   <td>Desarrollo
   </td>
   <td>El desarrollo se realiza a través de una comunidad colaborativa, generalmente no hay una empresa que controle el software
   </td>
   <td>El desarrollo puede ser realizado tanto por una comunidad como por una empresa privada
   </td>
  </tr>
  <tr>
   <td>Beneficios
   </td>
   <td>Proporciona libertad y flexibilidad a los usuarios finales
   </td>
   <td>Fomenta la innovación y el avance del software al permitir que un gran número de personas colaboren y contribuyan al proyecto
   </td>
  </tr>
  <tr>
   <td>Ejemplos de software
   </td>
   <td>Linux, GNU, Firefox, Apache, LibreOffice, etc.
   </td>
   <td>MySQL, Perl, Python, etc.
   </td>
  </tr>
</table>



## **Sistemas operativos y distribuciones**

Una distribución de Linux es una variante de Linux creada por una organización o comunidad específica que toma el kernel de Linux y lo combina con otras aplicaciones y herramientas de software para crear un sistema operativo completo. Las distribuciones de Linux pueden variar en características, propósitos y enfoques.

Hay muchas distribuciones de Linux disponibles, y algunas de las más populares son:

**Rolling Release:**

*Arch Linux \
*Gentoo \
*Solus \
*Manjaro \
*openSUSE Tumbleweed

**Fixed Release:**

*Debian \
*Ubuntu \
*CentOS \
*Fedora \
*Red Hat Enterprise Linux (RHEL)

Las **distribuciones de Rolling Release** reciben actualizaciones continuas y no tienen versiones específicas. Las actualizaciones se entregan a medida que se lanzan y se prueban. 

Las **distribuciones de Fixed Release**, por otro lado, tienen una versión específica que se lanza en un momento determinado y reciben actualizaciones de seguridad y mantenimiento regulares, pero no se actualizan con nuevas características de forma regular.


## **¿Dónde viven Servidores?**

Las ventajas que tenemos con un servicio en la nube, bien sea como persona natural o como empresa, es ahorrar dolores de cabeza con daños en los discos duros, tener preocupación por realizar copias de seguridad de los archivos de forma constante, y preocupación por recuperación de datos. \
los servicios en la nube, son realmente eficientes y tienen herramientas con gran poder que nos facilita mucho la vida.



* Alojamiento: \
**On Premise: ** Todo el hardware y software del servidor es alojado y mantenido por la organización. \
**Cloud: **Es una empresa que ofrece la arquitectura y estructura, y yo solo me encargo de administrar el servidor. o Nube Pública: o Nube Privada: Todos los servicios pueden estar en otro lugar, pero los recursos utilizados por una empresa no pueden ser compartidos con otra empresa, por ejemplo, un disco duro dedicado alojar datos de la empresa. \
**Hibrid (Hídrida):  **Es una combinación de los servicios premise y cloud. Data Center: lugar para almacenar servidores.


## Formas de montar un servidor

🚀 Hay varias formas de montar un servidor Linux, dependiendo de las necesidades y recursos de cada organización. Algunas de las formas comunes de montar un servidor Linux son las siguientes:



1. Servidores físicos: Consiste en instalar Linux en un servidor físico en las instalaciones de la organización. Este enfoque puede ser más adecuado para organizaciones que tienen un alto nivel de control sobre el hardware y la seguridad del servidor.
2. Servidores virtuales: Consiste en instalar Linux en una máquina virtual que se ejecuta en un servidor físico. Este enfoque puede ser más adecuado para organizaciones que necesitan flexibilidad y escalabilidad, pero que no tienen los recursos para adquirir y administrar un servidor físico.
3. Servidores en la nube: Consiste en instalar Linux en un servidor virtual alojado en la nube de un proveedor de servicios en la nube. Este enfoque puede ser más adecuado para organizaciones que desean acceso remoto, escalabilidad y flexibilidad sin tener que administrar su propio hardware.
4. Contenedores: Consiste en utilizar tecnología de contenedores para alojar aplicaciones en Linux. Los contenedores pueden ser más eficientes que las máquinas virtuales porque comparten recursos de hardware, lo que significa que pueden alojar más aplicaciones en un solo servidor.
5. Kubernetes: Consiste en utilizar una plataforma de orquestación de contenedores como Kubernetes para gestionar y escalar contenedores en un clúster de servidores Linux.

Cada uno de estos enfoques tiene sus propias ventajas y desventajas, y la elección depende de las necesidades específicas de la organización, como la escalabilidad, la flexibilidad y el control sobre el hardware y la seguridad del servidor.


## **Instalar Virtualbox en Linux 🐧**


### **Si tú, como yo, eres usuario Ubuntu te dejaré una pequeña guía de cómo instalarlo.**

(Si utilizas otra distribución, puedes expandir este aporte con tu distribución y cómo instalar virtualbox).



1. Primer paso, debes dirigirte a la página oficial de [VirtualBox](https://www.virtualbox.org/).
1. Debes darle click al botón gigante que te aparece para instalar VirtualBox y te redirige a otra página.

Nota: es muy importante tener en cuenta que si tu país no cumple con los requisitos políticos para adquirir servicios de Oracle, te recomiendo utilizar una VPN para poder descargar este programa. (🇻🇪🇨🇺🇳🇮)

Una vez estándo en la lista, debes elegir la opción que dice: Linux distributions



1. Ahí podemos observar una lista de distribuciones y debemos elegir la distribución que tengamos; en mi caso es Ubuntu y su versión es la 22.04
1. Debemos esperar a que el archivo se descargue.
2. Una vez descargado el archivo, en este caso es un archivo “deb”. Esto quiere decirnos que el gestor de paquetes que utilizamos es el mismo que el de Debian (deb) entonces podemos hacer la instalación gráfica con click e instalar o por la terminal. Tú decides cuál crees que te sea más fácil.
1. Para instalarla de forma gráfica, solamente debes pulsar _click derecho > abrir con otra aplicación > Instalar software_ Y te abrirá una forma gráfica de instalar.

7.1. O también la puedes instalar por la terminal con este comando \
`sudo dpkg -i virtualbox-7.0 \
`Por supuesto el nombre del paquete debe de ser idéntico a como está descargado.


#### **Espero les sirva y les sea de mucha utilidad. 👍**


## **Instalar Ubuntu Server ISO**

[https://ubuntu.com/download/server](https://ubuntu.com/download/server)

Usar Virtual Box


## **Error 1 al instalar**

vbo error kernel driver not installed (rc=-1908) virtualbox

solución:

actualizamos el sistema

**sudo apt-get update \
sudo apt-get upgrade**

instalamos los paquetes esenciales del kernel

**sudo apt-get install build-essential**

instalamos las cabeceras del kernel

de nuestro kernel que nos lo indica con :** uname -r**

**sudo apt-get install linux-headers-$(uname -r)**

limpiamos

**sudo apt autoremove**

ejecutamos la autoconfiguración de vbox como administrador

**sudo /sbin/vboxconfig**

Y ya tenemos todos los problemas resueltos


## **Configuración básica para un servidor remoto**

Comandos: \
ssh: lo usamos para confirmar que tengamos instalado openssh en el sistema, en caso de no estar instalado podemos instalarlo con el comando:


```
sudo apt install openssh
```


Para el caso de ubuntu server, o para el caso de RHEL con el comando:


```
sudo dnf install openssh
```


systemctl status sshd : Para verificar que el proceso de ssh este activo y corriendo en el sistema (si no les funcione agréguenle la palabra sudo al principio del comando para abrirlo con permisos de superusuario)

ip address : nos da datos sobre nuestros dispositivos de red, incluyendo la IP interna del servidor.

Ahora, para conectarse al servidor desde un dispositivo en la misma red, se puede usar el comando:


```
ssh username@localip
Ejemplo:
ssh username@192.168.1.53
```


Desde la PowerShell de Windows o la consola del sistema operativo que estés usando. \
 \
EXTRA

En caso de querer acceder remotamente a un servidor, el comando es el mismo, solo que ahora en vez de usar la ip local se usaría la IP pública, la cual se puede ver desde un navegador en internet buscando myip estando conectado a la misma red del servidor o desde el servidor usando algún comando como lo puede ser el siguiente:


```
curl ifconfig.me
```


Es importante tener en cuenta que para poder tener este acceso, se debe tener abierto a la red el puerto de internet número 22, adicionalmente es una buena práctica utilizar un firewall para que solo ciertas IPs puedan conectarse al servidor y así evitar accesos no autorizados.


---


# **💻 Manejo de Recursos Servidor Linux**

**El SO es almacenado en memoria**

**Revisión de hardware:** Esto lo hace la Bios o la UEFI, si la memoria, discos, procesador está correcto y pueda cargar el S.O.

**Selección del dispositivo de arranque:** Priorización del Sistema, selecciona la partición (si tenemos múltiples discos).l

**Detección de la partición EFI:** Se encarga de Detectar la partición del S.O. 

Carga del boot loader: Es el Carga Arranque del Sistema (si tenemos múltiples sistemas S.O. Ubuntu, RedHat u otros), arranque del bootloader es para Linux. 

**Determina el kernel a usar:** Hay diferentes versiones de Kernel por eso de bed e determinar que kernel se debe utilizar. 

**Carga del kernel**:

**Se carga el primer proceso (PID1):** Va a cargar el primer proceso PID1.

**Ejecuta scripts de inicio: **Los Script de inicio , servicios de terceros, actualización software correcta. u otros.

**Inicia el sistema:** inicia ventana Login.


## **Firmware del sistema**



* Hace un inventario y chequeo de todos los dispositivos conectados al sistema al momento del arranque (discos, memorias, etc.)
* Este a su vez crea interfaces para que el software del sistema operativo pueda usar estos dispositivos.


## **Boot Loader** 

Separa el firmware del sistema y el arranque del sistema operativo. Es un paso previo a que se ejecute el sistema operativo. 

Es útil para correr el SO en forma de rescate o con parámetros extra, t**ambien se utiliza en modo recovery**, y se puede iniciar el dispositivo con parámetros extra a nivel de kernel o boot loader.

Es el boot loader **(GRUB: the GRand Unified Boot loader)** por defecto en la mayoría de distribuciones Linux. Actualmente contamos con dos versiones: ● GRUB Legacy ● GRUB 2


## **BIOS:**

**UEFI:**

Utiliza un Sistema de particiones,  para ordenar las particiones, y si puede ser modificada por S.O. superior.

Entre los beneficios del modo de inicio UEFI sobre el modo de inicio Legacy BIOS, se incluyen: Compatibilidad para particiones de unidades de disco duro superiores a 2 Tbytes. Compatibilidad para más de cuatro particiones por unidad. Inicio rápido.


## **Resumen:**

Cuando se enciende un ordenador, la **BIOS **se ejecuta y verifica que todos los componentes estén funcionando correctamente. Cuando termina el chequeo, busca la partición de arranque (**bootloader**). Éste se encarga de cargar el sistema operativo en la **RAM **del ordenador. En el caso de **Linux**, **GRUB **es el bootloader más común.

Una vez que el **bootloader **ha cargado el sistema operativo, lo primero que se ejecuta es el **kernel**, que es el encargado de administrar los recursos del sistema. Cuando el **kernel **ha cargado, se ejecuta **Init**, que es el primer proceso que realiza el sistema operativo. Este se encarga de iniciar todos los procesos necesarios para el correcto funcionamiento del sistema operativo.

Luego, cuando el **sistema operativo** ha cargado sus procesos, se carga el entorno gráfico, que es la **interfaz **que los nosotros como usuarios vemos y con la que interactuamos.
