11) Deshacer el último commit (perdiendo los cambios realizados en el working copy)
¿Qué comando utilizaste en el paso 11? ¿Por qué?
Utilicé el comando:	"git reset --hard HEAD~1"
De esta manera me muevo al commit anterior y al mismo tiempo recupero en mi working copy los archivos tal como estaban en este commit.

12) Rehacer el último commit (el que acabamos de deshacer)
¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Utilicé los comandos: "git reflog" para poder encontrar el commit deshecho y "git reset --hard 353faf2" para moverme al commit.

13) Hacer un merge con ‘master’ (styled absorbe a master)
El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
No causo conflicto y tampoco se realizo el merge porque el commit en el que está la rama master es el commit padre entonces en la rama styled ya se tienen todos los cambios.

19) Hacer un merge de “htmlify” en “styled” (styled absorbe a htmlify)
El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Si causo conflicto debido a que en la rama styled y en la rama htmlify se realizaron cambios sobre el mismo archivo en las mismas lineas.

21) Desde “master”, hacer un merge con “styled”
El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
No causo ningun conflicto debido a que la rama styled ya tiene todos los commits de la rama master por lo cual se realiza un fast-forward moviendo el puntero de la rama master hasta el commit en el que se encuentra el puntero de la rama styled

25) Dibujar el diagrama
¿Qué comando o comandos utilizaste en el paso 25?
git log --graph --oneline --decorate

26) Hacer un merge “no fast-forward” de “title” en “master” (master absorbe a title)
El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Si se podria debido a que la rama title tiene todos los commits de la rama master.

27) Deshacer el merge (sin perder los cambios del working copy)
¿Qué comando o comandos utilizaste en el paso 27?
Utilicé el comando: "git reset HEAD~1"

28) Descartar los cambios
¿Qué comando o comandos utilizaste en el paso 28?
Utilicé el comando: "git checkout -- git-nuestro.md"

29) Eliminar la rama “title”
¿Qué comando o comandos utilizaste en el paso 29?
Utilicé el comando: "git branch -D title"

30) Rehacer el merge que hemos deshecho
¿Qué comando o comandos utilizaste en el paso 30?
Utilicé los comandos: "git reflog" para poder encontrar el merge y "git reset --hard e0462a2" para mover el puntero de la rama master al commit donde se realizo el merge.

32) Volver al commit inicial cuando se creó el poema
¿Qué comando o comandos usaste en el paso 32?
Utilicé los comandos: "git log" para buscar buscar el primer commit y "git checkout 5aa6a2fcb17136620fc6bf5a02cd1595b859fc45" para volver a este commit

33) Volver al estado final, cuando pusimos título al poema
¿Qué comando o comandos usaste en el punto 33?
Utilicé el comando: "git reset --hard HEAD@{1}" para desacer el comando anterior que era cuando me encotraba en el commit donde el poema tiene titulo.