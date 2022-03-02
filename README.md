# Hyperblog
Un incleible blog para el curso de git y github

####   **Notas del curso**

- git reset (codigo del commit) --hard
> vuelve a la versión anterior borrando el ultimo commit

- git checkout (numero del commit)
> ver la primera versión

- git checkout (rama)
> devuelve el head a la rama que necesito 

- git rm 
> borra archivos sin eliminar su historial del sistema de versiones
    **uso**
    - git rm --cached
	Elimina los archivos de nuestro repositorio local y del área de staging, pero los mantiene en nuestro disco duro
    - git rm --force
	Elimina los archivos de Git y del disco duro.

- git reset
> volvemos al pasado sin la posibilidad de volver al futuro. Borramos la historia y la debemos sobreescribir
    **uso**
    - git reset --hard
	borra toda la informacion de staging por siempre
    - git reset --soft
	Borramos todo el historial y los registros de Git pero guardamos los cambios que tengamos en Staging
    - git reset HEAD
	sacar archivos del área de staging. No para borrarlos ni nada de eso, solo para que los últimos cambios de estos archivos no se envíen al último commit                         

- git commit -am "mensaje"
> para subir los cambios sin decir git add

- alias arbol="git log --all --graph --decorate --oneline"
> sirve para ver los commit de forma grafica

- cambiar email global desde el home
> git -config --global user.email "email.gmail.com"

- crear llave ssh desde el home
	**pasos**
	1. **Crear**
> ssh-keygen -t rsa -b 4096 -C "dprueba20@gmail.com"
	1. **Verificar**
> eval $(ssh-agent -s)
	1. **Aregar la llave ssh**
> ssh-add ~/.ssh/id_rsa
	1. **cambiar http por ssh**
> git remote set-url origin (url del proyecto ssh)

- historial de las ramas a detallegit
> git show-branch --all

- git stash 
> sirve para guardar de manera temporal los cambios que no se pueden subir aun, devuelve los cambios al ultimo commit

- git stash list
> para ver el lugar temporal

- git stash pop
> Devuelve los cambios que se habian echo

- git stash branch nombre rama
> guardar cambios temporalmente en una nueva rama

- git clean --dry-run
> simula lo que se va a borrar sin borrarlo 

- git clean -f
> borra todos los archivos que concidere innecesarios
> *git clean solo borra las cosas que puede indexar*

- cherry-pick has o numero de commit
> traer un commit de otra rama, (es una mala practica)

- mezcla cambios nuevos al commit anterior
   ** uso**
>  1. git add carpeta/archivo
>  1. git commit --amend 

- git reflog 

- git grep palabra
> buscar palabras por consola

- git grep color
> cuantas veces he usado la palabra buscada

- git log -S "cabecera"
> buscar en la historia de los commits

*los archivos binarios no se deberian agregar al repositorio*

*abrir en windows archivo de wsl*
*explorer.exe .*
file://wsl.localhost/Ubuntu-20.04/home/daniela/MyCourser/Proyecto1/blogpost.html
https://pandao.github.io/editor.md/en.html

*Este readme.md esta diseñado para el ejemplo. Aunque las notas si van como corresponden *