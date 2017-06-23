# Respuestas a las preguntas de la practica.

- �Qu� comando utilizaste en el paso 11? �Por qu�?

  **git reset --hard HEAD~1**. Esta orden deshace el �ltimo commit y con el modificador --hard tambi�n deshacemos el working copy dejando todo como estaba. 

- �Qu� comando o comandos utilizaste en el paso 12? �Por qu�?

  **git reset --hard d47e37**. Con el comando git reset y utilizando el identificador del commit al que queremos ir, podemos mover el master y el head a dicho commit y recuperar el working copy que ten�amos en ese momento. 

- El merge del paso 13, �Caus� alg�n conflicto? �Por qu�?

    Cuando realizaos el merge, en este caso, obtenemos el mensaje Already up-to-date ya que la rama styled ya contiene el trabajo de la rama master que estamos intentando mergear.

- El merge del paso 19, �Caus� alg�n conflicto? �Por qu�?

    En este caso si tenemos un conflicto ya que el fichero git-nuestro de la rama styled es diferente al que tiene la rama htmlify y necesitamos resolver estos conflictos antes de seguir con el merge.

- El merge del paso 21, �Caus� alg�n conflicto? �Por qu�?

    No existe ning�n conflicto. Cuando realizamos del merge con styled, esta rama es la que tiene los �ltimos cambios realizados en el fichero git-nuestro.md. As� que simplemente realiza un merge fast forward de la master hacia styled.

- �Qu� comando o comandos utilizaste en el paso 25?

   **git log --graph --decorate --pretty=oneline**. De esta manera podemos ver el diagrama de manera gr�fica, en una l�nea y con todas las etiquetas en caso de tenerlas.

- El merge del paso 26, �Podr�a ser fast forward? �Por qu�?

   Si podr�a ser fast forward ya que simplemente la rama master apuntar�a al mismo commit que la rama title absorbiendo los cambios.

- �Qu� comando o comandos utilizaste en el paso 27?

   **git reset HEAD~1**

- �Qu� comando o comandos utilizaste en el paso 28?

   **git checkout -- git-nuestro.md**

- �Qu� comando o comandos utilizaste en el paso 29?

   **git branch -D title**

- �Qu� comando o comandos utilizaste en el paso 30?

  **git reset --hard f2dc0ff**

- �Qu� comando o comandos usaste en el paso 32?

  **git checkout b922adb** -Uso un checkout para moverme al commit inicial a trav�s de su hash. Genero un estado de detached HEAD pero me permite recuperar el working copy de ese momento. 

- �Qu� comando o comandos usaste en el punto 33?

  **git checkout ad7e1bc** - Utilizo la l�gica del punto anterior. La idea es practicar la navegaci�n por el grafo sin mover la rama con git reset.