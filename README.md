### Escuela Colombiana de Ingeniería
### Procesos de Desarrollo de Software
### Introducción a GIT

Trabajo en grupos (grupos de cuatro o cinco)


1. (Grupo 1) Clonar el proyecto actual.

2.	En cada grupo, crear una cuenta en GitHUB. En una de las dos cuentas, cree un nuevo repositorio. Invite al usuario del otro grupo como colaborador de dicho proyecto.

3. (Grupo 1) Haga 'push' del proyecto recién clonado al nuevo repositorio.

	```bash
	git push URL_REPOSITORIO master
	```

4. (Grupo 1) Agregue al libro, como autores, los integrantes del grupo (sólo el primer nombre). Agregue los cambios para el siguiente commit, haga commit, y haga 'push' de dichos commits:

	```bash
	git add .
	git commit -m "AUTORES DEL GRUPO 1 AGREGADOS"
	git push URL_REPOSITORIO master
	```

5. (Grupos 1 y 2) Revisen, a través del cliente Web de GitHUB, que el documento haya sido actualizado.

6. (Grupo 2) Clone el proyecto actualizado:

	```bash
	git clone URL_REPOSITORIO
	```

7.	(Grupo 2) Agregue los autores de su grupo al libro (sólo el primer nombre). Agregue los cambios para el siguiente commit, haga commit, y haga 'push' de dichos commits:

	```bash
	git add .
	git commit -m "AUTORES DEL GRUPO DOS AGREGADO"
	git push URL_REPOSITORIO master
	```

5. (Grupo 1) 'Jale' los 'commits' realizados por el grupo anterior, y revise que los mismos hayan sido aplicados al documento.
	
	```bash
	git pull URL_REPOSITORIO master
	```

6. (Grupos 1 y 2 al tiempo)

* Grupo 1: Remueve el paréntesis de la línea 5 de la fe de erratas.
* Grupo 2: Arregla los errores de ortografía.
* Grupo 1 y 2: Agreguen los cambios a sus repositorios locales, hagan commit y push. Los dos grupos lo pudieron hacer?, qué quedó al final en la versión oficial?

Si para alguno no es posible (por consistencia) hacer el ‘push’, haga antes un pull a la rama ‘master’ del repositorio en GitHub con ‘rebase’:

```bash
git pull --rebase URL_REPOSITORIO master
```

