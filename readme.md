Aaron Méndez Estrada

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
	--> $ git reset --hard HEAD~1
	--> Con el --hard evitamos hacer el restore más adelante, en ese caso queremos deshacer todos los cambios sin tener en cuenta nada, así    que la mejor opción es "reset --hard". Con HEAD aquí especificamos deshacer solamente 1 cambio.
	
	
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
	--> $ git reflog
	--> $ git reset --hard f505383
	--> Con el git reflog visualizamos todas las actualizaciones de las ramas entre otras, buscamos el identificador del paso 11 y lo
		reseteamos a ese identificador para deshacer todos los cambios hasta "f505383" (en mi caso).
		
		
- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
	--> No, ya que mientras estaba en la rama styled, no se subió nada al respositorio de la rama master (ningun commit).
	
	
- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
	--> Sí, hay conflicto, ya que la rama styled se ha fusionado con una rama que ha hecho un commit, por lo que el contenido del archivo
		readme.md son diferentes.
	
	
- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
	--> No, ya que los 2 archivos tienen las mismas lineas de código.
	
	
- ¿Qué comando o comandos utilizaste en el paso 25?
	--> $ git log --graph
	
	
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
	--> Sí, porque no se ha hecho ningún commit de la branca master cuando estaba en la otra.
	
	
- ¿Qué comando o comandos utilizaste en el paso 27?
	--> $ git reset HEAD~1
	
	
- ¿Qué comando o comandos utilizaste en el paso 28?
	--> $ git reset --hard e78e8bc
	--> Utilizando git reflog y analizando el comportamiento de las brancas, he hecho un reset al identificador del paso anterior.
	
	
- ¿Qué comando o comandos utilizaste en el paso 29?
	--> $ git branch -D title
		Deleted branch title (was 0f5c3b7).
	
	
- ¿Qué comando o comandos utilizaste en el paso 30?
	--> $ git reset --hard 0f5c3b7
		HEAD is now at 0f5c3b7 Titulo añadido branca title (archivo git-nuestro)
	
	
- ¿Qué comando o comandos usaste en el paso 32?
	--> $ git checkout 8113d51aa5731c4deff115128ac4d81e130964f9
	
	
- ¿Qué comando o comandos usaste en el punto 33?
	--> $ git checkout master