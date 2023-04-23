# Servidores-Linux-Ubuntu-Readme-DM

Apuntes de Configuracion de **Servidor en Linux**, todos las distribuciones probadas, Ububtu server.

- Autor: Alexander Jair Rojas Paria
--------------

# 📱 [Servidores Linux](https://platzi.com/cursos/linux/)


## **Roles de un Administrador**


#### **Habilidades clave:**



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
