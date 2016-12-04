- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
git reset --hard HEAD~1
Deshace el último commit y lo que había en mi working copy de manera que todo quede como estaba antes nuestro straging area queda vacío
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
git reflog observo todo lo que ha pasado,
git reset 1d4c5e1 para volver que hemos desecho, lo comprobamos con git log y vuelve aparecer el archivo modificado
- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
git merge master, porque estamos en style y absorbemos a master
- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
git checkout styled para pasar a la rama
git merge htmlify se crea un conflicto porque el archivo esta modificado en las dos ramas.
notepad git-nuestro.md se edita archivo y nos quedamos con lo de la rama styled
git add git-nuestro.md
git commit -m "añado archivo con conflicto quedándonos el texto de styled paso 9"
git merge htmlify ya no hay conflictos
- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
git checkout master
git merge styled
- ¿Qué comando o comandos utilizaste en el paso 25?
git log --graph –decorate
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
git merge --no-ff title
- ¿Qué comando o comandos utilizaste en el paso 27?
git checkout 7fb63969af7fbf20c25ebc66faef90d95904f716
Voy al anterior commit que era “añado archivo con titulo paso 23”
- ¿Qué comando o comandos utilizaste en el paso 28?
git reset HEAD~1
Para deshacer el merge no fast-forward
- ¿Qué comando o comandos utilizaste en el paso 29?
git branch -d title
- ¿Qué comando o comandos utilizaste en el paso 30?
Git reflog (buscamos el commit “merge title: Merge made by the 'recursive' strategy.”)
git checkout eb98e8e
- ¿Qué comando o comandos usaste en el paso 32?
Git reflog (buscamos el commit “añado git-nuestro al repositorio”)
git checkout 6065d06
- ¿Qué comando o comandos usaste en el punto 33?
Git reflog (buscamos el commit “añado archivo con titulo paso 23”)
git checkout 7fb6396
