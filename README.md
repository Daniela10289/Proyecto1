# Proyecto1
Curso de git y github

git reset (codigo del commit) --hard: vuelve a la version anterior borrando el ultimo commit

abrir en windows archivo de wsl
explorer.exe .
file://wsl.localhost/Ubuntu-20.04/home/daniela/MyCourser/Proyecto1/blogpost.html

git checkout (numero del commit): ver la primera version 
git checkout (rama): devuelve el head a la rama que necesito 

git rm: borra archivos sin eliminar su historial del sistema de versiones
    uso
    git rm --cached: Elimina los archivos de nuestro repositorio local y del área de staging, pero los mantiene en nuestro disco duro
    git rm --force: Elimina los archivos de Git y del disco duro.

git reset:  volvemos al pasado sin la posibilidad de volver al futuro. Borramos la historia y la debemos sobreescribir
    uso
    git reset --hard: borra toda la informacion de staging por siempre
    git reset --soft: Borramos todo el historial y los registros de Git pero guardamos los cambios que tengamos en Staging
    git reset HEAD: sacar archivos del área de staging. No para borrarlos ni nada de eso, solo para que los últimos cambios de estos archivos no se envíen al último commit                         

git commit -am "mensaje": para subir los cambios sin decir git add