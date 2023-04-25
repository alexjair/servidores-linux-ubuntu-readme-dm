# Servidores-Linux-Ubuntu-Readme-DM

Apuntes de Configuracion de **Servidor en Linux**, todos las distribuciones probadas, Ububtu server.

- Autor: Alexander Jair Rojas Paria
--------------

<!-- Output copied to clipboard! -->

<!-----

You have some errors, warnings, or alerts. If you are using reckless mode, turn it off to see inline alerts.
* ERRORs: 0
* WARNINGs: 0
* ALERTS: 12

Conversion time: 4.798 seconds.


Using this Markdown file:

1. Paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β34
* Mon Apr 24 2023 20:15:18 GMT-0700 (PDT)
* Source doc: Servidores Linux
* Tables are currently converted to HTML tables.
* This document has images: check for >>>>>  gd2md-html alert:  inline image link in generated source and store images to your server. NOTE: Images in exported zip file from Google Docs may not appear in  the same order as they do in your doc. Please check the images!


WARNING:
You have 7 H1 headings. You may want to use the "H1 -> H2" option to demote all headings by one level.

----->


<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 0; WARNINGs: 1; ALERTS: 12.</p>
<ul style="color: red; font-weight: bold"><li>See top comment block for details on ERRORs and WARNINGs. <li>In the converted Markdown or HTML, search for inline alerts that start with >>>>>  gd2md-html alert:  for specific instances that need correction.</ul>

<p style="color: red; font-weight: bold">Links to alert messages:</p><a href="#gdcalert1">alert1</a>
<a href="#gdcalert2">alert2</a>
<a href="#gdcalert3">alert3</a>
<a href="#gdcalert4">alert4</a>
<a href="#gdcalert5">alert5</a>
<a href="#gdcalert6">alert6</a>
<a href="#gdcalert7">alert7</a>
<a href="#gdcalert8">alert8</a>
<a href="#gdcalert9">alert9</a>
<a href="#gdcalert10">alert10</a>
<a href="#gdcalert11">alert11</a>
<a href="#gdcalert12">alert12</a>

<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>



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


## **¿Qué son los sistemas de archivos?**

En Linux, un sistema de archivos es la estructura que se utiliza para organizar y almacenar datos en dispositivos de almacenamiento, como discos duros, unidades flash USB, CD-ROM y otros dispositivos de almacenamiento.

El sistema de archivos determina cómo se organizan los datos en un dispositivo de almacenamiento y cómo se accede a ellos. En un sistema de archivos típico, los datos se organizan en archivos y directorios (también llamados carpetas), que se pueden acceder y manipular mediante comandos en la línea de comandos o mediante una interfaz gráfica de usuario.

Linux admite varios sistemas de archivos, incluidos los siguientes:



* **Ext4:** Es el sistema de archivos predeterminado en la mayoría de las distribuciones de Linux modernas. Es conocido por su rendimiento y confiabilidad.
* Btrfs: Es un sistema de archivos de alta tecnología diseñado para manejar grandes conjuntos de datos y proporcionar una alta redundancia y escalabilidad.
* **XFS:** Es un sistema de archivos de alto rendimiento que es adecuado para sistemas de archivos muy grandes.
* **NTFS**: Es un sistema de archivos utilizado en sistemas operativos Windows, pero que también puede ser utilizado en Linux.
* **FAT32**: Es un sistema de archivos compatible con muchos sistemas operativos y es utilizado comúnmente en unidades flash USB y otros dispositivos de almacenamiento portátiles.

Cada sistema de archivos tiene sus propias características y ventajas, y la elección del sistema de archivos adecuado depende de las necesidades y requisitos específicos de cada caso de uso.


## **Particiones de un Servidor Linux**

**df: (Disk Free)** en Linux se utiliza para mostrar información sobre el espacio en disco utilizado y disponible en el sistema de archivos. Cuando se ejecuta el comando “df” sin argumentos, se muestra una lista de todas las particiones montadas en el sistema junto con su uso de espacio y su capacidad total. \
Algunos de los argumentos más comunes que se utilizan con el comando “df” son:



* **-h:** muestra la información de uso de espacio en formato legible por humanos, lo que significa que muestra la capacidad y el espacio utilizado en unidades como GB, MB, KB, etc., en lugar de bytes.
* **-T:** muestra el tipo de sistema de archivos en lugar del tipo de dispositivo.
* **-i:** muestra información sobre el uso de inodos en lugar de bloques.
* **-t:** muestra solo las particiones que coinciden con el tipo de sistema de archivos especificado.

**El comando lsblk **en Linux se utiliza para listar información acerca de los dispositivos de almacenamiento del sistema, incluyendo discos duros, unidades flash USB, tarjetas SD, particiones, entre otros.

Cuando se ejecuta el comando **lsblk **sin argumentos, muestra una lista jerárquica de los dispositivos de almacenamiento conectados al sistema, incluyendo el tamaño, el nombre del dispositivo y el tipo de partición. También muestra información acerca de cómo los dispositivos están conectados al sistema, como los controladores SCSI, SATA o USB.

Linux lista los discos como sda: sda, sdb, sdc, etc. Estos discos se pueden particionar a nivel logico y cada particion va a estar enumerada: sda1, sda2, sdb1, sdb2

Algunos de los argumentos más comunes que se utilizan con el comando lsblk son:



* **-a:** muestra todos los dispositivos, incluso aquellos que no están en uso o no tienen sistemas de archivos asociados.
* **-f: **muestra información adicional sobre los sistemas de archivos asociados con cada dispositivo.
* **-n**: suprime la cabecera y muestra solo la lista de dispositivos en una columna.
* **-o:** permite al usuario especificar qué columnas deben mostrarse en la salida.

. \
**El comando fdisk **en Linux se utiliza para crear, editar y administrar particiones en el disco duro de un sistema. Con **fdisk**, se pueden ver las particiones existentes, crear nuevas particiones, modificar sus tamaños, tipos y formatos de sistema de archivos. Además, **fdisk **permite realizar otras tareas, como imprimir la tabla de particiones, verificar la integridad de las particiones, o escribir una tabla de particiones en un archivo. \
. \
La partición swap en Linux es un área de almacenamiento temporal en el disco duro que se utiliza cuando se agota la memoria RAM del sistema. Permite al sistema operativo manejar eficientemente los recursos de memoria y actúa como una extensión de la memoria RAM. Es importante asignar un tamaño apropiado a la partición swap para evitar un uso excesivo que pueda perjudicar el rendimiento del sistema.


## **Manejo de un archivo swap**

Una muy buena practica antes de editar archivos de linux es el de crear un backup antes de modificarlo (por si algo sale mal, podemos regresar rapido a como estaba antes) e.g.:

**sudo cp /etc/fstab /etc/fstab.bak**

Con eso ya tendremos un archivo backup si llegamos a necesitarlo (que si que podemos llegar a hacerlo)

CREAR TU MEMORIA SWAP

Es la memoria auxiliar a disco duro o archivo (swap.file), es para emergencias.

**Requisitos:**

Ingresar al modo (Mover al ROOT) de Ubuntu Server:

**cd /**

Confirmar si tengo un archivo swap actualmente: debe de existir el **swap.img**

**ls -lh**

Ver la **cantidad de memoria** disponible (Men: | Swap: )

**free -h**

Ver si tengo suficiente espacio en disco para aumentar la particion swap actual o crear una nueva:

**df -h**

**Creación Memoria Auxiliar:**

Creo un archivo especial para mi memoria swap


```
sudo fallocate -l 2G /swapfile

```



* **2G: **Tamaño de memoria a adicionar. (2 Gigabytes).
* /**swapfile: **Nombre del archivo de uso para la memoria.

Verificar los, configurar **permisos **para que solo el root acceda a este archivo acceda en lectura y escritura

**sudo chmod 600 /swapfile**



* Permisos de solo lectura y escritura para root 600.

Confirmo que tengo mi archivo swap creado

**ls -lh**

Convertir el archivo swap creado en un archivo swap valido

**sudo mkswap /swapfile**

Configurar el archivo swapfile para que cuando se reinicie el sistema siga con la configuración: Configurar el fstab

**sudo vim /etc/fstab**

**EDITAR CON VIM: **

Escribir nueva linea en el archivo fstab, abajo de /swap.img

**/swapfile swap swap defaults 0 0**



* 0: Zero para evitar el respaldo xq es una memoria volátil.
* 0: Evita la revisión de disco xq es una memoria volátil.
1. Para salir de vim solo teclea **ESCAPE **luego **:wq** y dar ENTER,el archivo se guarda y sales del editor

Comprobar los cambios que hice al archivo fstab: 

**cat /etc/fstab**

**free -h **(Ver nuestra memoria, antes de aplicar los cambios)

Activamos nuestro archivo especial como memoria swap:

**sudo swapon /swapfile**

**Remover la memoria Swap (cuando la nmo la necesite)**

Si queremos desactivar nuestro archivo para ya no usarlo como memoria swap solo usamos: 

**sudo swapoff /swapfile**

**free -h **(Ver el estado nuestra memoria)

Eliminar la linea del archivo fstab que configuramos anteriormente.

Remover la linea del archivo VIM

**sudo vim /etc/fstab**

Se quita con doble “dd” o borrado &lt;--

**/swapfile swap swap defaults 0 0**

**free -h **(Ver el estado nuestra memoria)

Solo falta eliminar el archivo (con cuidado es RM)

**sudo rm swapfile**

ver el archivo

**ls -lh**


## **Árbol de directorios**

🚀 El árbol de directorios en Linux es una estructura jerárquica de directorios y archivos que se utiliza para organizar y almacenar datos en un sistema operativo Linux. Este árbol de directorios comienza en el directorio raíz, representado por una sola barra (/), y se extiende a través de una serie de subdirectorios que se organizan en función de su función y contenido.

**ls /--carpeta--/**

**ll /run/**

*/**bin**: Contiene archivos binarios ejecutables esenciales para el sistema. \
*/**boot**: Contiene los archivos necesarios para arrancar el sistema. \
*/**dev**: Contiene archivos de dispositivos que representan hardware y otros dispositivos del sistema. \
*/**etc**: Contiene archivos de configuración del sistema. \
*/**home**: Contiene los directorios personales de los usuarios. \
*/**lib**: Contiene bibliotecas compartidas necesarias para los programas del sistema. \
*/**media**: Contiene puntos de montaje para dispositivos extraíbles, como unidades flash USB y discos duros externos. \
*/**mnt**: Contiene puntos de montaje para sistemas de archivos temporales o permanentes. \
*/**opt**: Contiene programas y archivos adicionales del sistema. \
*/**proc**: Contiene información en tiempo real sobre el sistema y los procesos en ejecución. \
*/**root**: El directorio personal del usuario “root”. \
*/**run**: Contiene archivos de estado del sistema y otros archivos temporales. \
*/**sbin**: Contiene archivos binarios ejecutables esenciales para el sistema. \
*/**srv**: Contiene datos de servicio para servidores web y otros servicios de red. \
*/**sys**: Contiene archivos de dispositivos virtuales que representan hardware y otros dispositivos del sistema. \
*/**tmp**: Contiene archivos temporales. \
*/**usr**: Contiene programas y archivos no esenciales del sistema. \
*/**var**: Contiene datos variables del sistema, como registros y archivos de caché. \
En general, el árbol de directorios en Linux está diseñado para proporcionar una estructura coherente y fácil de entender para el almacenamiento y la organización de datos del sistema, lo que hace que sea más fácil administrar y mantener sistemas Linux.


## **Diferentes tipos de archivos**

Tipos de permisos



<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image1.jpg "image_tooltip")
 \
Permisos y atributos



<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image2.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image2.jpg "image_tooltip")
 \
Permisos en sistema de archivos



<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image3.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image3.jpg "image_tooltip")



## **¿Qué es un manejador de paquetes?**

Un manejador de paquetes en Linux es un programa que se utiliza para instalar, actualizar, configurar y eliminar paquetes de software en un sistema Linux. Los manejadores de paquetes se encargan de todo el proceso de gestión de paquetes, desde la descarga del software hasta su instalación y eliminación.

Algunos de los manejadores de paquetes más comunes en Linux incluyen:



* **APT **(Advanced Package Tool): utilizado en distribuciones basadas en Debian, como Ubuntu y Linux Mint.
* **YUM **(Yellowdog Updater Modified): utilizado en distribuciones basadas en Red Hat, como Fedora y CentOS.
* **DNF **(Dandified YUM): utilizado en distribuciones basadas en Red Hat, como Fedora y CentOS (a partir de CentOS 8).
* **Zypper**: utilizado en distribuciones basadas en SUSE, como openSUSE y SUSE Linux Enterprise.
* **Pacman**: utilizado en Arch Linux y distribuciones derivadas de Arch.

Cada manejador de paquetes tiene su propio conjunto de comandos y opciones para realizar diferentes tareas, como instalar, actualizar o eliminar paquetes de software. Los manejadores de paquetes son una parte fundamental del ecosistema de software de Linux, y permiten a los usuarios gestionar el software de una forma más fácil y segura.


## **Manejador de paquetes**

Para usar APT en Ubuntu o Linux Mint, puedes utilizar los siguientes comandos:

Listar los paquetes en Ubuntu:

**apt list**

Listar los paquetes instalados en el sistema:

**apt list --installed**

Ejemplo: 

Realizamos la instalación de una vaca :3 

**sudo apt install cowsay -y**

Probando el paquete instalado:

**cowsay hola**

Actualizar la lista de paquetes disponibles en los **REPOSITORIOS**: \
**sudo apt update**

Actualizar todos los paquetes instalados en el sistema del repositorio: \
**sudo apt upgrade**



* Despues te pregunta si vas a reiniciar los servicios actualizados, pones que si, **“Ok”**

Instalar un paquete en espesifico:

**sudo apt install &lt;nombre_del_paquete>**

Eliminar un paquete: \
**sudo apt remove &lt;nombre_del_paquete>**

Buscar un paquete en los repositorios: \
**apt search &lt;nombre_del_paquete>**

Para usar DNF en Fedora o CentOS 8 (o versiones posteriores), puedes utilizar los siguientes comandos:



* Actualizar la lista de paquetes disponibles en los repositorios: \
s**udo dnf update**
* Instalar un paquete: \
**sudo dnf install &lt;nombre_del_paquete>**
* Actualizar todos los paquetes instalados en el sistema: \
**sudo dnf upgrade**
* Eliminar un paquete: \
**sudo dnf remove &lt;nombre_del_paquete>**
* Buscar un paquete en los repositorios: \
**sudo dnf search &lt;nombre_del_paquete>**

Ambos manejadores de paquetes tienen muchas más opciones y comandos disponibles, pero estos son algunos de los más comunes y útiles para empezar a trabajar con ellos.


## **¿Cómo instalar software?**

En Linux, es común instalar software desde la línea de comandos utilizando el manejador de paquetes de la distribución que estés utilizando. El proceso para instalar un paquete es bastante sencillo y se realiza en unos pocos pasos:



1. Actualiza la lista de paquetes disponibles en los repositorios utilizando el siguiente comando:
    * En distribuciones basadas en Debian, como **Ubuntu o Linux** Mint, utiliza: \
**sudo apt update**
    * En distribuciones basadas en Red Hat, como Fedora o CentOS, utiliza: \
**sudo dnf update**
2. Busca el paquete que quieres instalar utilizando el comando de búsqueda correspondiente:
    * En distribuciones basadas en **Debian**, utiliza: \
**apt search &lt;nombre_del_paquete>**
    * En distribuciones basadas en Red Hat, utiliza: \
**dnf search &lt;nombre_del_paquete>**
3. Una vez que encuentres el paquete que quieres instalar, utiliza el comando correspondiente para instalarlo:
    * En distribuciones basadas en Debian, utiliza: \
**sudo apt install &lt;nombre_del_paquete>**
    * En distribuciones basadas en Red Hat, utiliza: \
**sudo dnf install &lt;nombre_del_paquete>**
4. Espera a que se complete la instalación del paquete. En algunos casos, se te pedirá que confirmes la instalación o que **ingreses tu contraseña de administrador**.

Y eso es todo, ahora deberías tener el paquete instalado en tu sistema Linux y listo para ser utilizado. Ten en cuenta que, dependiendo del paquete que estés instalando, es posible que necesites reiniciar ciertos servicios o aplicaciones para que los cambios tengan efecto.

Repositorios Online:



* En snapcraft.io
* Ejemplo: **<code>sudo snap install nvim --classic</code></strong>
* para verificar. <strong>nvim </strong>(enter)
* Salir de vim: <strong>“:q”</strong>

Para saber las capacidades de un sistema linux:



* **sudo apt install screenfecth**
* Luego aceptar el reinicio de servicios afectados. (x)
* Para ver: **screenfecth**


## **Manejo de repositorios**

Aqui hay otra expresion regular para listar los repositorios en Ubuntu:

**grep -E '^deb' /etc/apt/sources.list**



* La opción** “-E”** permite usar una expresión regular extendida y el símbolo **^** indica el comienzo de una línea.

Para listar los repositorios:

**cat /etc/apt/sources.list**

Listar con expresion regular los paquetes

**grep ^[^#] /etc/apt/sources.list**

<span style="text-decoration:underline;">Hay repositorios Universe y Multiverse</span>


    Añadir los repositorios multiverse (con esto podremos agregar mas software):


    **sudo add-apt-repository multiverse** 


    Actualizar los repositorios:


    **sudo apt update**


## **¿Qué es un proceso en Linux?**

 Linux Process States

[https://www.baeldung.com/linux/process-states](https://www.baeldung.com/linux/process-states)

Lista de Procesos - y la descripción

[https://www-uxsup.csx.cam.ac.uk/courses/moved.Building/signals.pdf](https://www-uxsup.csx.cam.ac.uk/courses/moved.Building/signals.pdf)


### Daemon (Demonio)

En Linux, un demonio (daemon) es un programa que se ejecuta en segundo plano para realizar tareas que no requieren la intervención del usuario o que se deben realizar de forma continua, como la gestión del sistema, el monitoreo de servicios o la automatización de tareas.


### Ejemplos comunes:



* Servidores web
* Servidores de bases de datos
* Servicios de correo electrónico.

Nosotros podemos interactuar y comunicarnos con los procesos a través de señales. Hay varias señales, y cada señal tiene un propósito diferente. Para enumerar todas las señales posibles, podemos ejecutar, como usuario root, el comando

kill -L


## Escaneo de procesos

Para escanear un proceso en Linux, puedes utilizar varias herramientas, como **ps, top, htop, pgrep, pidof**, entre otras. A continuación, te mostraré algunos ejemplos con los comandos **ps y top**.

Para escanear un proceso utilizando el comando **ps**, simplemente debes ejecutar el siguiente comando en la terminal:

**ps aux | grep nombre_del_proceso**



* Donde **nombre_del_proceso **es el nombre del proceso que deseas escanear. Este comando mostrará una lista de procesos que coinciden con el nombre especificado.

Para ordenar que procesos estan usando mas CPU con top se puede usar el comando:

**top -o %CPU**

Para ver cual esta usando mas memoria ram se puede hacer algo similar:

**top -o %MEM**

Para mostrar los Pid de los procesos, (ejm. less)

**pidof --nombre-proceso--**

**pidof less**

Para listar todos los archivos de socket, por el puerto que se ejecutan: 

**lsof**

**man lsof  **(Informacion)

Para mostrar los procesos en un puerto:

**sudo lsof -i :22 **

Ver los procesos con información en caliente

**top**

**htop  **(versión mejorada)



<p id="gdcalert4" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image4.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert5">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image4.png "image_tooltip")



## **Manejo de procesos**

Estados de un proceso:



* **R**: Running or Runnable
* **D**: Un interruptible Sleep (No puede ser interrumpido de forma sencilla: kill …)
* **S:** Interruptible Sleep (Es facil de interrumpir)
* **T:** Stopped (Pausado)
* **Z:** Zombie ()

Correr un proceso en 2do plano:

**less espera.txt &  **(el operador & es para indicar que se va ejecutar en 2do plano)

**less espera.txt **( proceso en 1er plano | normal inicio)

Para ver los procesos en 2do plano: (background)


```
jobs -l

```



* **<code>[1]+ 1391 Stopped (tty output) less espera.txt</code></strong>

Para traer al fairground:

**fg 1 **

Para matar un proceso

**kill 1402**

**kill {PID}**

Para para proceso en la en el background

**kill -s SIGKILL 1478 **

**kill -s SIGKILL {PID}**

Para matar a todos los procesos, todos los asociados a el

**killall less**

**killall {nombre-proceso}**

<span style="text-decoration:underline;">Tabla de kill</span>

**kill &lt;OPTION> &lt;PID>  **   

**kill -9 1425**

# Envia una señal al proceso con el ID especificado, por defecto SIGTERM

-1             # SIGHUP, reinicia el proceso

-2             # SIGINT, interrumpe el proceso

-9             # SIGKILL, termina el proceso de manera forzosa (backgroup)

-15            # SIGTERM, termina el proceso de manera normal &lt;opción por defecto>

-19            # SIGSTOP, pausa el proceso

-18           # SIGCONT, reanuda el proceso


## **Creación y manejo de demonios**

Ver el 1er demonio proceso que usa: se encarga de controlar los servicios de sistema, red, gráficos. si creamos un proc. demon se debe agregar a los demon, 

**man systemd**

Manejo de systemd

**man systemctl**

Se crea un ejemplo en python.py


<table>
  <tr>
   <td><strong><code>import time</code></strong>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong><code>from datetime import datetime</code></strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong><code>while True:</code></strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong><code>   with open("/datelogs/timestamp.txt", "a") as f:</code></strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong><code>       f.write("\nTimestamp: " + str(datetime.now()))</code></strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong><code>       f.close()</code></strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><code>   time.sleep(1)</code>
   </td>
  </tr>
</table>


se guarda con VIM en linux

ahora debemos ingerar con root, porque el demon debe de ejecutarse, en la carpeta root para que se ejecute parta todos los usuarios.

entrar como root

**su root**

No emos configurado el usuario root, se debe agregar la contraseña.

**sudo passwd**

se ingresa al root:

**su root**

Ingresar a la carpeta root

**cd /**

Ver los archivos de root:

**ls**

crear una carpeta datelogs y scripts

**mkdir datelogs**

**mkdir scripts**

Entrar a scripts

**cd scripts/**

Crear el archivo py (el ejm. arriba)

**vim logger.py**

Ejecutar el scripts

**python3 logger.py**

Para ver el contenido en otra terminal.

**cat /datelogs/timestamp.txt**

**cat /datelogs/{nombre-archivo.txt}**


## **Scripts como Servicio (Demons)**

Para ejecutar el scripts en cada inicio de sistema.

Ir al carpeta:

**cd /etc/systemd/system**

Para ver los archivos 

**ls -l**

Ver un servicio. demon ejemplo como se estructura: 

**cat snap.lxd.user-daemon.service**


    _alexjair@ubuntuserver:/etc/systemd/system$ **cat  snap.lxd.user-daemon.service**_


    _[Unit]_


    _# Auto-generated, DO NOT EDIT_


    _Description=Service for snap application lxd.user-daemon_


    _Requires=snap-lxd-24322.mount_


    _Wants=network.target_


    _After=snap-lxd-24322.mount network.target snapd.apparmor.service_


    _X-Snappy=yes_


    _[Service]_


    _EnvironmentFile=-/etc/environment_


    _ExecStart=/usr/bin/snap run lxd.user-daemon_


    _SyslogIdentifier=lxd.user-daemon_


    _Restart=on-failure_


    _WorkingDirectory=/var/snap/lxd/24322_


    _TimeoutStopSec=600_


    _Type=simple_


    _Delegate=true_

Procedemos a crear el servicio:(debe de tener permisos de root)

**vim loggerpython.service**

Escribir el script:


    [Unit]


    Description=A python date logger


    After=**multi-user.target**


    [Service]


    Type=**simple**


    Restart=**Always**


    ExecStart=**/usr/bin/python3 /scripts/logger.py**


    [Install]


    WantedBy=**multi-user.target**

El “ExecStart=**/usr/bin/python3 /scripts/logger.py**” se puede cambiar los archivos Shell, Bash, o otro python. 

El “After=**multi-user.target**”, para iniciar el servicio al prender el sistema.

El “Restart=**Always**”, siempre debe de ejecutarse.

Para iniciar el serv.demon reiniciar el systemd

**systemctl daemon-reload**

Pero aun no está iniciado…

ver el servicio

**systemctl status loggerpython.service**

**systemctl status {nombre-archivo-servicio.service}**

Enviar para q se inicie al incio del sistema

**systemctl enable loggerpython.service**

**systemctl **enable **{nombre-archivo-servicio.service}**

Otra terminal

Hay que eliminar para este ejemplo el archivo .txt donde se graba las horas.

**sudo rm /datelogs/timestamp.txt**

Ahora sí iniciar el demos,service

**systemctl start loggerpython.service**

**systemctl start** **{nombre-archivo-servicio.service}**


    _root@ubuntuserver:/etc/systemd/system# **systemctl status loggerpython.service**_


    _● loggerpython.service - A python date logger_


    _     Loaded: loaded (/etc/systemd/system/loggerpython.service; enabled; vendor preset: enabled)_


    _     Active: active (running) since Mon 2023-04-24 02:27:34 UTC; 1min 7s ago_


    _   Main PID: 2934 (python3)_


    _      Tasks: 1 (limit: 2234)_


    _     Memory: 3.5M_


    _        CPU: 48ms_


    _     CGroup: /system.slice/loggerpython.service_


    _             └─2934 /usr/bin/python3 /scripts/logger.py_


    _abr 24 02:27:34 ubuntuserver systemd[1]: Started A python date logger._


    _root@ubuntuserver:/etc/systemd/system#_

Parar el daemon.service, pero no del inicio de sistema.

**systemctl stop loggerpython.service**

Parar el inicio y sistema.

**systemctl disable loggerpython.service**


## **Automatización de procesos con cron job**

Usar root para crear los Cron Job, para que use a lo largo del sistema.

ver si esta activo el cron job.

**systemctl status cron**

Configuración

**crontab -e** 



* selecciona el numero 2 para el ejemplo.

[https://ostechnix.com/a-beginners-guide-to-cron-jobs/](https://ostechnix.com/a-beginners-guide-to-cron-jobs/) (guia)

En otra terminal ejecutar, para ver los ejemplos de crontap

**less /etc/crontab**



<p id="gdcalert5" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image5.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert6">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image5.png "image_tooltip")


Continuar editando el crontap:


    **0 3 * * 0 	apt update && apt upgrade**


    espacio|espacio|espacio|espacio|tap|espacio|espacio|espacio|espacio|

El cron, el cron daemon lo está leyendo y ejecutando. por defecto.

Ver mi crontap del usuario actual

**crontab -l**

Editar el contrab del usuario actual.

**crontab -e**

ver mi cron status 

**systemctl status cron**


---


# 💻 Manejo de Recursos Servidor Linux


# **Arranque del sistema**

**El SO es almacenado en memoria**

**Revisión de hardware:** Esto lo hace la Bios o la UEFI, si la memoria, discos, procesador está correcto y pueda cargar el S.O.

**Selección del dispositivo de arranque:** Priorización del Sistema, selecciona la partición (si tenemos múltiples discos).l

**Detección de la partición EFI:** Se encarga de Detectar la partición del S.O. 

Carga del boot loader: Es el Carga Arranque del Sistema (si tenemos múltiples sistemas S.O. Ubuntu, RedHat u otros), arranque del bootloader es para Linux. 

**Determina el kernel a usar:** Hay diferentes versiones de Kernel por eso de bed e determinar que kernel se debe utilizar. 

**Carga del kernel**:

**Se carga el primer proceso (PID1):** Va a cargar el primer proceso PID1.

**Ejecuta scripts de inicio: **Los Script de inicio , servicios de terceros, actualización software correcta. u otros.

**Inicia el sistema:** inicia la ventana Login.


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


## **Grupos y Usuarios en Linux**

**Usuario:** \
Nos permite separar las responsabilidades y permisos de acciones en el sistema. Dependiendo los permisos que tengan son las acciones que podrán ejecutar.

**Características:** \
	- UID: Identificador único del sistema \
	- GIDs: uno o más IDs que los relacionan a un grupo \
Directorio Home: 

está en la ruta 

**/home/&lt;username>** \
Archivos 

**/etc/passwd:** contiene info de nuestros usuarios en formato **name:password:UID:GID:GECOS:directory:shell** \
	- GECOS: info extra \
	- SHELL: la shell de inicio \


**/etc/shadow**: contraseña de forma cifrada.



* Si contiene un asterisco ***** significa que jamas tuvo una contraseña asignada
* Si contiene un símbolo de exclamación **!** ha sido bloqueado

Grupos: Agrupan usuario y conjunto de permisos, estos son muy usados por servicios como demonios, docker, postgres, etc


# **Grupos y usuarios**


## **Manejo Usuarios en Linux**

Con el comando se bloquee a un usuario:

**usermod --lock user**

**ls**: listar directorio actual

**ls /home:** listar un directorio específico

**if config:** Configuración de red

Conexión por ssh

**ssh alexjair@192.168.1.57** 

Ver los usuarios

**cat /etc/passwd:** ver archivo donde estan los usuarios

**less /etc/shadow**: ver usuarios con su contraseña de forma cifrada

**sudo** **less /etc/shadow **(Modo root) (podemos usar tanto less o cat)

press “q” para salir

Manejo de Usuarios

Solo el Usuario Root puede agregar usuarios.

**su root**: cambiar a usuario admin

**pwd**: nombre del directorio actual

Agregar usuario;

**adduser username**: agregar nuevo usuario

**adduser {--Nombre-usuario--}**



* Ejemplo: **adduser fulano**
* Agrega el Password:
* y Completa la información.

**whoami:** ver usuario actual logueado.

Ver la info usuario

**id:** ver info del usuario (uid,gid,groups)

**id -u**

**id -um**

Ingresamos como root:

**su root**

Cambiamos de otros usuario:

**chfn {username}:** cambiar información del usuario

ver la info. de usuario

**less /etc/passwd**

iniciar la sesión SHH con fulano

**ssh fulano@192168.1.53**

Bloquear a uusario

**usermod --lock username**: bloquear usuario (accesos futuros)

ver si se bloqueo fulano

**cat /etc/shadow**

terminar el bloqueo o desbloquear

**usermod --unlock {username}** 

Ver procesos para kill el proceso ssh de Fulano

**htop:** ver todos los procesos actuales (podemos ver los procesos referentes a un usuario) 

	ubicamos el proceso.

→con **F9 **matamos el proceso



<p id="gdcalert6" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image6.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert7">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image6.png "image_tooltip")


 \
Por ejemplo los que aparecen con ssh

**sudo deluser username**: eliminar un usuario (aunque la carpeta en home permanece)

**sudo deluser {username}**

**rm -rf /home/username/**: eliminar un directorio como la carpeta del usuario

Ver los usuarios que tengo

**ls /home**


## **Manejo de grupos**

Para manejar grupos de usuarios en Linux, se pueden seguir los siguientes pasos:



1. Verificar los grupos existentes: se puede usar el comando 

    **cat /etc/group** 


    para mostrar una lista de los grupos existentes en el sistema.

2. Crear un nuevo grupo: se puede utilizar el comando 

    **sudo groupadd &lt;nombre_del_grupo>** 


    para crear un nuevo grupo en el sistema.

3. Agregar usuarios a un grupo: se puede utilizar el comando 

    **sudo usermod -a -G &lt;nombre_del_grupo> &lt;nombre_de_usuario>** 


    para agregar un usuario existente al grupo.

4. Verificar los usuarios de un grupo: se puede utilizar el comando 

    **id &lt;nombre_del_grupo>** 


    para mostrar una lista de usuarios que pertenecen a un grupo.

5. Eliminar un grupo: se puede utilizar el comando 

    **sudo groupdel &lt;nombre_del_grupo>** 


    para eliminar un grupo existente en el sistema.

6. Cambiar los permisos de un archivo o directorio para un grupo: se puede utilizar el comando 

    **sudo chgrp &lt;nombre_del_grupo> &lt;ruta_al_archivo_o_directorio>** 


    para cambiar el grupo propietario de un archivo o directorio. Luego se puede utilizar el comando 


    **sudo chmod g+&lt;permisos> &lt;ruta_al_archivo_o_directorio>** 


    para otorgar permisos específicos para el grupo propietario.

7. Cambiar el nombre de un grupo: se puede utilizar el comando** sudo groupmod -n &lt;nuevo_nombre> &lt;nombre_actual>** para cambiar el nombre de un grupo existente.
8. Verificar los permisos de un grupo: se puede utilizar el comando 

    **sudo getfacl /ruta/al/archivo-o-directorio** 


    para verificar los permisos de un archivo o directorio. En la salida del comando, se puede observar información sobre los permisos de usuario, grupo y otros.

9. Agregar usuarios a un grupo secundario: se puede utilizar el comando 

    **sudo usermod -a -G &lt;nombre_del_grupo_secundario> &lt;nombre_de_usuario>** 


    para agregar un usuario existente a un grupo secundario.

10. Eliminar usuarios de un grupo: se puede utilizar el comando 

    **sudo gpasswd -d &lt;nombre_de_usuario> &lt;nombre_del_grupo>** 


    para eliminar un usuario existente de un grupo.

11. Verificar los permisos de un grupo específico: se puede utilizar el comando sudo visudo para abrir el archivo de configuración sudoers, y luego agregar la siguiente línea para permitir que los usuarios del grupo tengan permisos de superusuario: **%&lt;nombre_del_grupo> ALL=(ALL) ALL**.
12. Verificar los grupos de un usuario: se puede utilizar el comando 

    **groups &lt;nombre_de_usuario>** 


    para mostrar una lista de grupos a los que pertenece un usuario específico.


Manejo:

Archivo de los grupos, para ver en:

**less /etc/group**

buscar que usuario está en que grupo,alexjair

**less /etc/group | grep codevars**

Ver los grupos donde estoy, si mi sesión está iniciada.

**groups**

Ver todos los usuarios que pertenecen a SUDO

**getent group {-nombre-del-grupo}**

**getent group sudo**

<span style="text-decoration:underline;">Manejo de Grupos</span>:

Crear un grupo:

**groupadd {nombre_grupo}**

**groupadd amigos**

Ver los grupos

**less /etc/group**

Modificar nombre de Grupo

**groupmod -n {name-new} {name-antiguo}**

**groupmod -n friends amigos **

Acceder usuario root para evitar el password

**su root**

ver los cambios

**cat /etc/group**

Crear carpeta compartida con los usuarios

agregar un nuevo usuario -fulano

**adduser fulano**

**adduser perengano**

Acceder al home como fulano

**su fulano**

**cd**

**pwd (para ver si estamos en el home)**

**groups**

Crear un grupo que tenga acceso a la carpeta compartida

Logger como root y crear la carpeta “shared”

**mkdir shared**

Ver los archivos.

**ls -l**

Ver en qué grupo está, en los detalles y hay que cambiar el **owner**

CAmbiar de Owner a la carpeta shared

**chgrp friends /shared/**

CAmbiar los permisos de directorio

**chmod {per.ucuario}{per.grupo}{per.otros} /{carpeta-name}/**

**chmod 770 /shared/**

ver como quedo 

**ls -l**

Agregar que el grupo realice acciones especiales, esto es para que cualquier archivo que cree en ese folder conserve su permisos del grupo

**chmod +s /shared**

Agregar usuarios a este grupo(aG: addGroup)

**usermod -aG {name-grupo} {name-user}**

**usermod -aG friends fulano**

**usermod -aG friends perengano**

Ingresar como fulano

**su fulano**

ver sus grupos

**groups**

crear un mensaje en la carpeta /shared

**echo “hola soy fulano” > mesage.txt**

si se creo en otra carpeta por error: se debe de cambiar la carpeta 

**mv mesage.txt /shared**

Ingresar con perengano

**su perengano**

ver el archivo compartido

**cat /shared/mesage.txt**

Ahora eliminar grupo y permisos

iniciar con root:

**gpasswd -d {-name-user-} {name-group}**

**gpasswd -d perengano friends**

verificar si esta en el grupo de friends

**getent group {name-group}**

**getent group friends**

Eliminar el grupo de amigos (friends)

**groupdel {name-group}**

**groupdel friends**

Verificar grupos, ver si se eliminó

**cat /etc/group**

Clase:

**<code>groupadd groupname</code></strong>: crear nuevo grupo

**<code>groupdel groupname</code></strong>: eliminar grupo

**<code>groupmod -n newGroupName oldGroupName</code></strong>: cambiar el nombre de un grupo

**<code>usermod -aG groupname username</code></strong>: agregar usuario existente a grupo existente

**<code>useradd username -m -g groupname</code></strong>: crear usuario y asignarlo a un grupo, -m crea el directorio personal y -g asigna el usuario a un grupo ya creado

**<code>gpaswd -d username groupname</code></strong>: quitar usuario de un grupo

**<code>mkdir shared</code></strong>: crear carpeta

**<code>ls -la</code></strong>: ver permisos de las carpetas

**<code>chgrp groupname /shared/</code></strong>: asignar carpeta a grupo

**<code>chmod 770 /shared/</code></strong>: cambiar permisos, todos los permisos al owner, todos al grupo y denegar acceso a todos los que no pertenezcan al grupo

**<code>chmod +s /shared/</code>:</strong> asignar permisos especiales, cualquier archivo que creemos dentro del directorio se va a crear con el group owner

**<code>less /etc/group | grep username</code></strong>: buscar usuario especifico dentro de los grupos

**<code>less /etc/group</code></strong>: listar grupos

**<code>ls</code></strong>: listar directorio actual

**<code>ls /home</code>:</strong> listar un directorio especifico

**<code>if config</code>:</strong> configuracion de red

**<code>ssh username@ip</code>:</strong> conexion por ssh

**<code>cat /etc/passwd</code>:</strong> ver archivo donde estan los usuarios

**<code>less /etc/shadow</code>:</strong> ver usuarios con su contraseña de forma cifrada (podemos usar tanto less o cat)

**<code>su username</code>:</strong> cambiarse de usuario

**<code>pwd</code></strong>: nombre del directorio actual

**<code>adduser username</code></strong>: agregar nuevo usuario

**<code>whoami</code></strong>: ver usuario actual

**<code>id</code></strong>: ver info del usuario (uid,gid,groups)

**<code>chfn username</code></strong>: cambiar informacion del usuario

**<code>usermod --lock username</code></strong>: bloquear usuario (accesos futuros)

**<code>htop</code></strong>: ver todos los procesos actuales (podemos ver los procesos referentes a un usuario) con F9 matamos el proceso por ejemplo los que aparecen con ssh

**<code>deluser username</code>:</strong> eliminar un usuario (aunque la carpeta en home permanece)

**<code>rm -rf /home/username/</code></strong>: eliminar un directorio como la carpeta del usuario


# **Control de accesos**


## **Control de accesos en Linux**

Linux todo lo ve como un objeto, el control de acceso depende del usuario

La cuenta **root **puede acceder a cualquier objeto. 

No acceder directamente a **root**, mejor usar **su**.

Dar permisos de administrador solo a los usuarios necesarios.

Revocar accesos de administrador después de cierto tiempo.


## **Creación de un usuario administrador**

Ingresar con el usuario perengano.

**su perengano**

Si queremos ver todos los usuarios 

**sudo cat /etc/passwd**



* No le dejara ver el archivo porque no tiene permisos de administrador

Agregar usuario como grupo adminitrador

Iniciar como root:

**su root**

Agregar a perengano a grupo sudo

**usermod -aG sudo perengano**

verificar si esta en el grupo sudo

**getent group sudo**

Ver el archivo suder, para ver que personas estan ahi.

**sudo less /etc/sudoers**

Para poder editar el archivo sudoers.

**sudo visudo**


# Almacenamiento


## **Particionando y montando una unidad**

Agregar un disco virtual de “Respaldo”



* Apagar la máquina virtual.
* Ve al virtual box, y a la sección de **Configuraciones -> Almacenamiento**
* Selecciona controlador SATA, luego icono “Añadir disco duro”
* Debe de seleccionar Disco -VDI
* Disco de tipo dinámico.
* Colocar 10GB, luego seleccionarlo.

Iniciar la maq. virtual

Conectarte como ssh

Para ver el disco duro

**lsblk**

saber donde se encuentra, y como acceder al nuevo disco

**fdisk -l**



<p id="gdcalert7" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image7.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert8">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image7.png "image_tooltip")


Nos colocamos en la partición

Para crear particiones, y vemos que estan en **/dev/sdb**

ver la herramiento fdisk

**sudo fdisk /dev/sdb**

para ver todas las opciones ingresa

**m** (menu)

listar los tipos particiones 

**l **(listar)

Para crear una nueva partición

**n** 

Escoge el typo:

**p**

Partition number: default 1 

**(enter)**

First Sector: default enter

**(enter)**

Last Sector, tamaño:

**+3G** (aquí le damos 3GB)

--se logro la partición 

para ver las particiones:

**p**

Crear una nueva partición n2 (7 Gigabytes)

**n** 

Escoge el typo:

**p**

Partition number: default 1 

**(enter)**

First Sector: default enter

**(enter)**

Last Sector, tamaño:

**+7G** (aquí le damos 3GB) o (enter) para que tome el resto

--se logro la partición 

para ver las particiones:

**p**

Se ve tenemos todas las particiones 

Para aplicar las particiones en el disco escribir:

**w**

salir del programa.

Formatear la partición

ver nuestras particiones

**lsblk**


    _Try: sudo apt install &lt;deb name>_


    _alexjair@ubuntuserver:~$ lsblk_


    _NAME   MAJ:MIN RM   SIZE RO TYPE MOUNTPOINTS_


    _loop0    7:0    0  53,2M  1 loop /snap/snapd/18933_


    _loop1    7:1    0  63,3M  1 loop /snap/core20/1822_


    _loop2    7:2    0  49,8M  1 loop /snap/snapd/18357_


    _loop3    7:3    0    73M  1 loop /snap/core22/607_


    _loop4    7:4    0  63,3M  1 loop /snap/core20/1852_


    _loop5    7:5    0  20,7M  1 loop /snap/nvim/2797_


    _loop6    7:6    0 111,9M  1 loop /snap/lxd/24322_


    _sda      8:0    0    25G  0 disk_


    _├─sda1   8:1    0     1M  0 part_


    _└─sda2   8:2    0    25G  0 part /_


    _sdb      8:16   0    10G  0 disk_


    _├**─sdb1   8:17   0     3G  0 part**_


    **_└─sdb2   8:18   0     7G  0 part_**


    _sr0     11:0    1  1024M  0 rom_

Para formatear una partición:

**mkfs.ext4 /dev/sdb1**

Ahora 

Montar la Unidad

Deben de ir al root

**cd /**

Crear un directorio “scripts” ahi vamos a montar la partición sdb1

**sudo mkdir scripts**

Montar la unidad

**sudo mount /dev/sdb1 /scripts**

**sudo mount {-dirección-partición-} {-directorio-donde -montar-}**

Ahora escribir un archivo en unidad

**sudo vim /scripts/hola.py**



* dentro del archivo: script(“hola mundo”)

ejecutar el script

**python3 /scripts/hola.py**

Desmontar el sistema de archivos

**sudo umount /dev/sdb1**

verificar si esta desmontado

**ls /scripts/**



* no muestra nada

Para montar de nuevo

**sudo mount /dev/sdb1 /scripts**

verificar

**ls /scripts/**

Montar nuestro file system al inicio del arranque de sistema.

**sudo vim /etc/fstab**



<p id="gdcalert8" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image8.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert9">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image8.png "image_tooltip")


para ver si realizo los cambios.

**sudo reboot **(reinicia el servidor)

“Si el filesystem no se guardó bien o no se editó correctamente, puedes entrar en modo recovery con super usuario y arreglarlo”

ver si se montó bien

**lsblk**

**ls /scripts**



<p id="gdcalert9" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image9.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert10">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image9.png "image_tooltip")



## ¿Qué es RAID y LVM?

**Raid** : 

Redundant Array of Independent Disks:

Permite crear un arreglo de discos para realizar redundancia, que si uno de nuestros discos se estropea los otros tienen una copia exacta.



<p id="gdcalert10" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image10.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert11">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image10.png "image_tooltip")


**LVM:**

Logical Volume Manager.

Monta sobre el mismo, en el “volumen lógico”, ahí donde trabaja crea sectores de 10GB o 5GB, varios discos volúmenes. Todos se trabajan sobre un dispositivo disco físico. 



<p id="gdcalert11" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image11.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert12">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image11.png "image_tooltip")



# **Proyecto 1: LVM sobre RAID 1**


## **Creación de sistema RAID 1**

Creamos 2 discos nuevos para los RAID de 5GB en el virtual Box, que se dinamico.



<p id="gdcalert12" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image12.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert13">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image12.png "image_tooltip")


Iniciamos nuestro servidor de ubuntu.
