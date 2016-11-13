# ¿Qué es Git?

Git es un sistema de gestión de versiones distribuido. Como el nombre lo indica, gestiona versiones de forma que cada consignación (commit) para a ser un hito en una línea de tiempo. Es así como cada vez que consignamos un cambio, este Git lo asocia con la consignación anterior. 

Todo esto se realiza dentro de un repositorio. Físicamente un repositorio es un directorio dentro del sistema operativo que consta de un subdirectorio llamado .git/ donde se almacena los detalles del mismo. Para crear un repositorio Git en nuestro sistema de archivos, hacemos los siguientes pasos:

```$ mkdir [directorio-de-repo]```
```$ cd [directorio-de-repo]```
```$ git init```

Con este sencillo paso hemos creado un repositorio local.

# Áreas de Git

Ahora bien, comprendamos la estructura de un repositorio Git. Git cuenta con 3 áreas que son:

* El área de trabajo
* El área de espera
* El repositorio

## Área de trabajo

Es el espacio donde editamos los archivos de nuestro proyecto. Aquí es donde agregamos, modificamos y borramos nuestros archivos.

## Área de espera

Una vez que realizamos nuestros cambios debemos indicar a Git que estos están listos para consignar. Para ello usamos el comando `git add [nombre-de-archivo]` (tenga en cuenta que git  permite usar atajos como el nombre de una carpeta para agregar todo su contenido o simplemente `git add .` para agregar todos los archivos de una sola vez)

Para ver que modificaciones están en el área de espera utilice el comando `git status`.

Para ver la diferencias de sus cambios con la versión anterior utilice el comando `git diff [nombre-de-archivo]`.

Para consignar los cambios al repositorio se utiliza el comando `git commit` (o alternativamente `git commit -m "su mensaje identificando los cambios"` )

## El repositorio

Es el área donde se almacenan todos los cambios consignafos en el proyecto. Al Git ser un gestor de versiones distribuido, usted tiene en su repositorio local una copia completa del historial del proyecto, con todos los cambios consignados.

Para ver el histórico de los cambios dentro del repositorio usaremos el comando `git log` y se le desplegará la lista de consignaciones con sus datos (entre ellos mensaje, usuario, fecha y hora, y huella digital del cambio).


