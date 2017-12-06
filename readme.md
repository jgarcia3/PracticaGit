# PracticaGit

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

Al estar en el branch Styled, he usado el comando git reset --hard HEAD~1
He usado este comando, ya que precisamente por especificar hard, elimino el contenido del working area

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

Primero realicé un git reflog para buscar en qué paso tenía el archivo que quería recuperar.
Posteriormente utilicé git checkout del hash(identificador) para ir directamente a ese archivo.
Luego lo asocié a una branch nueva para poder hacer un commit.
Luego hice merge con styled para devolver el archivo a la branch que le correspondía.
Finalmente, como ya no necesitaba la rama nueva, la borré usando git branch -d (en minúscula para que desaparezca totalmente)

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

En este caso el merge no causa ningún conflicto, ya que es la rama "hija" la que absorve al padre, y por lo tanto, la integra

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 

En este caso sí que existe conflicto, ya que la rama "padre" está abosrbiendo a la rama "hija" con el mismo archivo

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 

No hubo conflicto, directamente absorbió le branch styled y el archivo tanto en styled como en master es el mismo, el de styled

- ¿Qué comando o comandos utilizaste en el paso 25?

git log --graph --decorate --pretty=oneline

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 

No, ya que si fuera con fast forward habría conflicto

- ¿Qué comando o comandos utilizaste en el paso 27?

git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 28? 

git --abort

- ¿Qué comando o comandos utilizaste en el paso 29? 

git branch -d title

- ¿Qué comando o comandos utilizaste en el paso 30? 

git reflog

- ¿Qué comando o comandos usaste en el paso 32?

git reflog, y luego copia y pega del primer archivo que creé con el mensaje "He creado el primer archivo git-nuestro", y luego git checkout y el has (código corto)

- ¿Qué comando o comandos usaste en el punto 33?

exáctamente lo mismo que en el anterior, lo único que en este caso he buscado el has correspondiente al mensaje de "Añado titulo en la rama title"
