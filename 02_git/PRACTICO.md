# PRACTICO GIT


## DESCRIPCIÓN

En este tutorial veremos como crear e importar un proyecto a git, realizar algunos cambios y compartirlo con otros desarrolladores, es un tutorial muy introductorio que cubrirá las bases para manejarnos con git durante el curso. Si alguien esta interesado en profundizar en git para control de versiones le sugiero que revise el libro de git [Pro Git](https://git-scm.com/book) que tiene ejemplos y es de acceso libre.


## OBJETIVOS

1. Proveer al alumno conocimientos de control de versiones
2. Conocer los principales comandos de git


## PRÁCTICO

Comenzamos abriendo un terminal de git (lo que instalamos la semana pasada [aquí](README.md))

Luego ejecutaremos el comando que nos permite acceder a la ayuda de git

	git help log

Podremos ver que esta instruccion nos ayudara a ver los commits (ya veremos esto) realizados en nuestro proyecto y algunos parámetros para visualizar la información.

### Creación de un repositorio git

Crearemos un directorio nuevo donde le parezca más adecuado, por ejemplo, en windows podría ser ``C:/Usuarios/usuario/gitrepos/CURSO_ACI777`` donde usuario es su nombre de usuario en windows.

Si se encuentra en linux un buen directorio podría ser ``/home/usuario/gitrepos/CURSO_ACI777``

### :warning: Este repositorio será el que utilizaremos durante todo el curso y las evaluaciones las haré sobre los archivos que vayan dejando ahí de forma pública.

Luego nos vamos a ese directorio en la terminal de git

Windows:

	cd C:/Usuarios/usuario/gitrepos/CURSO_ACI777

linux:

	cd /home/usuario/gitrepos/CURSO_ACI777


Ahora inicializaremos o crearemos el repositorio en git:

	git init

Esto creara un directorio oculto llamado .git que contiene todo lo necesario para que el directorio se convierta en un repositorio git, sin embargo, todavía no hay seguimiento del repositorio.

Ahora crearemos un archivo readme dentro del directorio con su editor favorito, lo llamaremos README.md (md del formato [markdown](https://es.wikipedia.org/wiki/Markdown), [torpedo markdown](https://warpedvisions.org/projects/markdown-cheat-sheet/))

Dentro escribiremos lo siguiente 

	# Repositorio del Curso de Analisis de datos de la UDLA 2021 (nombre)

En mi caso nombre=dtravisany

	# Repositorio del Curso de Analisis de datos de la UDLA 2021 (dtravisany)

Ahora escribiremos:

	## Contenidos

	1. [Práctico de Git](01_practico_git/README.md)


Guardaremos el contenido y utilizaremos el comando ``status`` 

	git status

Veremos que nos dice que todavia no hay commits y nos sugiere que utilicemos el comando ``add``.

Entonces hemos aprendido que el comando `git status` nos muestra que archivos tienen y cuales no tienen seguimiento en nuestro repositorio.

Ahora utilizaremos el comando ``add``, podemos actualizar todo el directorio en el que me encuentro en el repo con . o agregar los archivos o carpetas de a uno, por ejemplo `git add .` o `git add README.md`. 

Utilizaremos

	git add .
	 
y ahora podemos volver a checkear con `git status`


	git status

y nos dice que hay cambios que deben ser confirmados

Para confirmar utilizaremos el comando `git commit` y le agregaremos un mensaje con el parámetro -m que haga una descripción corta de las modificaciones realizadas.

	git commit -m "Primer commit, se agrega README.md"

y veremos una descripción de lo que ha sucedido en nuestro repo.

Crearemos una carpeta nueva en el directorio

	mkdir 01_practico_git

y crearemos un archivo dentro de esa carpeta llamado `README.md`

luego nos devolveremos a la carpeta raíz del proyecto y haremos

	git add .
	git commit -m "Agregada carpeta y README para práctico git"


## :warning: Los siguientes comandos los veremos en el práctico de Github 


	


## DISCLAIMER

Este práctico ha sido elaborado a partir del tutorial oficial de git. 
Puede encontrarlo [acá](https://git-scm.com/docs/gittutorial).



