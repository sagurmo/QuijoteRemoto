# Práctica GIT

### Gurrea Moreno, Sara

# PracticaGit - Respuestas

--
**1. ¿Quécomando utilizaste en el paso 11?¿Por qué?**

`git reset --hard HEAD~1` 

Utilizamos este comando porque deshace tanto el commit como lo que hay en el working copy.

--

**2. ¿Qué comando o comandos utilizaste en el paso 12?¿Por qué?**

`git reflog` 

Vemos el historial de los comandos de modo que averiguamos el código del segundo commit que hemos hecho

`git reset —hard d3527f0` 

Recuperamos el commit

--

**3. El merge del paso 13,¿Causó algún conflicto?¿Por qué?**

`git merge master` 

Estando en style absorberíamos a Master, pero como Style está más adelantado que Master y ya lo incluye realmente no haría falta hacer un merge.

`git checkout styled` 

Nos pasamos a styled para poder absorber la otra rama

--

**4. El merge del paso 19,¿Causó algún conflicto?¿Por qué?**

`git checkout styled` 

Nos vamos a  la rama styled  para poder hacer el merge


`git merge htmlify ` 

Nos sale conflicto porque hemos unido dos cocumentos en uno solo, de modo que el último ha "machacado" el anterior. Arreglamos el documento y hacemos un nuevo commit.

--

**5. El merge del paso 21,¿Causó algún conflicto?¿Por qué?**

`git chekout master` 

Para irnos a la rama master


`git merge styled` 

Se hace un merge fast-forward, no hay conflicto, tan sólo nos indica que style ya contenía a master.

--

**6. ¿Qué comando o comandos utilizaste en el paso 25?**

`git graph` 

Con este comando se crea  el gráfico

--

**7. El merge del paso 26,¿Podría ser fast-forward?¿Por qué?**

`git checkout master` 

Para irnos a la rama master y desde ahí poder absorver a title.


`git merge title` 

Sí que puede ser fast-forward porque title se ha creado desde la rama master de modo que lo único que hemos hecho ha sido avanzar en la misma línea.

--

**8. ¿Qué comando o comandos utilizaste en el paso 27?**

`git reflog` 

Para ver el indicador del paso anterior al merge.


`git reset --hard 5daec3b` 

Para volver al paso anterior de crear el merge.

--

**9. ¿Qué comando o comandos utilizaste en el paso 28?**

Pregunta trampa. No podemos descartar los cambios porque no hemos hecho ningún cambio en el archivo, solo hemos creado el merge.

--

**10. ¿Qué comando o comandos utilizaste en el paso 29?**

`git checkout master` 

No podemos eliminar una rama en la cual estamos situados, por eso nos vamos a la rama master.


`git branch -d title` 

Borramos la rama desde master.

--

**11. ¿Qué comando o comandos utilizaste en el paso 30?**

`git reflog` 

Para encontrar el paso donde hemos hecho el merge del title.


`git reset --hard 52b972e` 

Volvemos al merge de title.

--

**12. ¿Qué comando o comandos utilizaste en el paso 32?**

`git reflog` 

Para encontrar el identificador del commit inicial.


`git reset --hard 69cdca7` 

Para volver al commit inicial “Subimos el primer texto al repositorio”.

--

**13. ¿Qué comando o comandos utilizaste en el paso 33?**

`git reflog` 

Para encontrar el identificador del paso donde pusimos el título al poema.


`git reset --hard 52b972e` 

Volvemos al commit “Añadimos título”.


