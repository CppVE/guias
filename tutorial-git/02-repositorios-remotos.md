# Repositorios Remotos

Como se dijo antes, Git es un sistema gestor de versiones distribuido, lo que quiere decir que podemos tener copias de nuestro proyecto en varias ubicaciones simultáneamente, con distintos cambios y diferentes personas trabajando en ello. Para realizar una copia de un repositorio (o proyecto) existente utilizamos el comando `git clone [ruta-al-repo-remoto] {ruta-local-al-repo}`, la ruta local al repo es un parámetro opcional, si no se coloca git creará un directorio con el nombre del repositorio original. La ruta al repositorio remoto es una URI que puede definir una carpeta dentro del mismo equipo, una ruta remota mediante el uso de ssh, una ruta http o https, o el protocolo git.

Ahora tiene un repositorio local y uno remoto (el cual ha clonado) [1]. Es así que usted tiene un repositorio remoto (digamos que en algún servicio de hospedaje de código como GitHub, GitLab o Bitbucket, o una carpeta remota), usted ha consignado localmente los cambios de una sesión de trabajo, ahora es momento de «subir» esos cambios a su repositorio remoto, para ello utilizamos el comando `git push`. Ahora bien, si usted tiene una copia local de su repo en otro equipo deberá entonces utilizar el comando `git pull` para incorporar los cambios de las consignaciones que acaba de registrar.

Es así como para realizar una copia local de un repositorio usamos el comando `git clone`, para enviar los cambios al repositorio remoto `git push` y para traernos los cambios `git pull`.

———
[1] En aras de desarrollar los conceptos esta explicación se concentrará en un repositorio utilizado por una sola persona, para ampliar en próximos capítulos
