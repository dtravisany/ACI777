# git

## ¿Qué es git?

Git es un sistema de [control de versiones](https://es.wikipedia.org/wiki/Control_de_versiones) 
pensado para ser rápido y eficiente. Ha sido diseñado para manejar proyectos pequeños o muy grandes.

Git es fácil de aprender y mantiene un buen performance.

Un sistema de control de versiones nos permite guardar distintas versiones del proyecto y tener un historial de modificaciones.
Algunas utilidades de git son:

 1. Revisar versiones anteriores.
 2. Volver a versiones anteriores.
 3. Ramificación de código para distintos desarrolladores.
 4. Es Open Source.
 5. [Otras](https://git-scm.com/about)




En este tutorial partiremos con la instalación de git.

## Instalación de git

### Para Linux :penguin: / OsX :apple: :
Podemos descargarlo desde [https://git-scm.com]

o podemos realizar la instalación con la herramienta [apt](https://wiki.debian.org/es/Apt) en Debian/Ubuntu
si contamos con los privilegios de [sudo](https://wiki.debian.org/es/sudo)

Abra una terminal y ejecute el siguiente comando:

	sudo apt-get install git

En red-hat based distro podemos realizar la instalación con [yum](https://access.redhat.com/es/solutions/238003) siendo sudo.

	sudo yum install git



### Instalación en Windows 


No hay una versión oficial de git para windows, sin embargo existe una herramienta llamada [git for windows](https://gitforwindows.org/)
que podemos utilizar para ejecutar git en windows. Git for windows provee de una emulación de [Bash](https://es.wikipedia.org/wiki/Bash) para ejecutar los comandos de git en sistema operativo Windows. Otra cosa que podemos agregar, es que git for windows, posee una interfaz gráfica de usuario.

Podemos descargar git for windows desde el siguiente repositorio oficial de [git-for-windows](https://github.com/git-for-windows/git/releases/)

#### Procederemos a descargar y ver paso a paso la configuración de git for windows.

1. Entramos a https://gitforwindows.org/ y descargamos la versión en el link download:

![DOWNLOAD](imgs/01descarga.png)

2. Una vez descargado hacemos click en el .exe y se nos abrirá el tipico wizard de instalación:  

![DESCARGADO](imgs/02descargado.PNG)  

3. Aceptamos la licencia [GNU General Public License Version 2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html):

![LICENCIA](imgs/03next1.PNG)

4. Seleccionamos el path donde queremos que sea instalado git for windows, como podemos ver en la imagen en esta versión deben existir por lo menos 263 MB disponibles de espacio en disco para instalar el software:

![PATH](imgs/04path.PNG)

5. Seleccionamos los componentes que queremos instalar, en mi caso yo agregue un acceso directo en el escritorio: 

![COMPONENTES](imgs/05selectcomp.PNG)

6. En esta ventana, seleccionamos el nombre del menú de inicio donde se agregaran los accesos directos:

![MENUFOLDER](imgs/06menufolder.PNG)

7. Ahora seleccionamos el editor de texto con el que vamos a trabajar en git.
#### :warning: Advertencia: en mi caso estoy acostumbrado a utilizar [Vim](https://www.vim.org/).
Vim es extremadamente útil sobretodo en entornos sin interfaz gráfica, pero resulta complejo adaptarse a utilizarlo y puede ser "tricky" dominarlo. 

:nerd_face: Como nota geek: El libro [Learning the Vi and Vim Editors](https://www.oreilly.com/library/view/learning-the-vi/9780596529833/) de O'REILLY dice: _"No hay nada por lo que los usuarios de Unix y Linux sean más fanáticos que su editor de texto. Los editores son objeto de adoración y culto, o de desprecio y burla..."_  

Como en recomendaciones anteriores, les sugiero el editor [Notepad++](https://notepad-plus-plus.org/), pero también [Atom](https://atom.io/), [Visual Studio](https://visualstudio.microsoft.com/es/) o [Sublime](https://www.sublimetext.com/).

![EDITORTEXTO](imgs/07etexto.PNG)

8. La siguiente configuración, la dejaremos como "git decide", que dejará por defecto el nombre: master:
 
![GITDECIDE](imgs/08gitdecide.PNG)

9. En lo relativo al ajuste de la variable __"PATH"__, dejaremos la recomendación del instalador, lo que evitará que ciertos comandos de bash se impongan sobre algunos comandos de Windows que son homónimos. 
![PATH2](imgs/09override.PNG)  
10. Utilizaremos la versión de [OpenSSH](https://www.openssh.com/) que viene por defecto con el instalador de git for windows, para no tener problemas de compatibilidad.  

![SSH](imgs/10ssh.PNG)  

11. Para el backend de transporte de HTTPS utilizaremos la biblioteca/librería [OpenSSL](https://www.openssl.org/)  

![OpenSSL](imgs/11ssl.PNG)  

12. El término de línea en Windows y Unix difiere, por lo que debemos seleccionar como vamos a tratar este asunto, mi sugerencia transformar el estilo de windows al estilo de unix al ejecutar los commit.  

![Termino de Línea](imgs/12lineending.PNG)  

13. Utilizaremos la terminal [MinTTY](https://mintty.github.io/) que es un emulador de la terminal de Unix y que presenta mejoras en relación a [cmd.exe](https://es.wikipedia.org/wiki/Símbolo_del_sistema) de Windows.  

![MinTTY](imgs/13window.PNG)  

14. Si recordamos, git pull, es el comando que nos permite actualizar nuestro repositorio local, dejaremos el comportamiento por defecto para git pull en git for windows.

![git pull](imgs/14gitpull.PNG)  

15. Credenciales de acceso, desde principios de agosto de 2021, github requiere un complejo sistema de autenticación, __Git Credential Manager Core__ nos ayudará a manipular las credenciales de acceso de forma simplificada para acceder a la nube.

![Credenciales](imgs/15credentials.PNG)  

16. Extras: Para mejorar la velocidad de algunas operaciones activaremos el sistema de caché, como se ve en la siguiente imagen:  

![CACHE](imgs/16extras.PNG)

17. Opciones Experimentales: Por ahora no activaremos opciones experimentales debido a que estamos recién aprendiendo a utilizar git y nos será muy difícil o casi imposible identificar si un problema con git viene desde nuestra interacción con la aplicación o es parte de problemas con la opción experimental.

![EXPERIMENTAL](imgs/17experimental.PNG)  

18. Ahora esperamos que termine el instalador...   

![Avance](imgs/18avance.PNG)  

19. Completamos la configuración de git y marcamos :check: donde está _Launch Git Bash_:  

![LAUNCH](imgs/19launch.png)  

20. Esto ejecutará MinTTY en nuestro entorno, ya tenemos git instalado y estamos listos para aplicar lo aprendido en la clase teórica.

![MinTTY](imgs/20terminal.PNG) 



## Ahora podemos continuar al práctico de [github](../03_Practico_github/README.md).







