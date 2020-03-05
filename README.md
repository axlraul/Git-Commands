Git Commands
============

_Lista de comandos comunmente utilizados_

--

### Descargando y Creando proyectos

| Comando | Descripción |
| ------- | ----------- |
| `git init` | Initializar local Git repository |
| `git clone ssh://git@github.com/[nombreusuario]/[nombre-repositorio].git` | Crear una copia local del respositorio remoot |

### Instantáneas, comentarios y adición

| Comando | Descripcion |
| ------- | ----------- |
| `git status` | comprobar estado del directorio de trabajo |
| `git add [nombrearchivo]` | Añade una instantánea del directorio de trabajo en el área de preparación |
| `git add -A` | Añade todos los cambios nuevos al área de preparación |
| `git commit -m "[Mensaje de ejecución]"` | Confirma una instantánea del directorio del entorno de ensayo en el historial de confirmaciones de los repositorios |
| `git rm -r [nombrearchivo]` | Borra un archivo o carpeta de la instanánea del directorio de trabajo |

### Ramas & Merging

| Comando | Descripción |
| ------- | ----------- |
| `git branch` | Lista todas las ramas (El asterisco denota la rama actual) |
| `git branch -a` | Lista todas las ramas (locales y remotas) |
| `git branch [nombre rama]` | Crea una rama nueva |
| `git branch -d [nombre rama]` | Borra una rama |
| `git push origin --delete [nombre rama]` | Borra una rama remota |
| `git checkout -b [nombre rama]` | Crear una rama nueva y cambiar a esta |
| `git checkout -b [nombre rama] origin/[branch name]` | Clonar una rama remota y cambiar a esta |
| `git branch -m [antiguo nombre de rama] [nuevo nombre de rama]` | Renombrar una rama local |
| `git checkout [nombre rama]` | Cambiar a una rama |
| `git checkout -` | Cambiar a la rama anteriormente utilizada |
| `git checkout -- [file-name.txt]` | Descartar los cambios realizados en un fichero |
| `git merge [nombre rama]` | Unir una rama en la rama actual |
| `git merge [rama fuente] [rama objetivo]` | Unir una rama en la rama objetivo |
| `git stash` | Reservar cambios en un directorio de trabajo temporal |
| `git stash clear` | Eliminar todas las entradas realizadas |

### Compartir & Subir Proyectos

| Comando | Descripción |
| ------- | ----------- |
| `git push origin [nombre rama]` | Subir una rama al repositorio remoto |
| `git push -u origin [nombre rama]` | Subir cambios al repositorio remoto (y recordar la rama) |
| `git push` | Subir cambios al repositorio remoto (rama recordada previamente) |
| `git push origin --delete [nombre rama]` | Eliminar una rama remota |
| `git pull` | Actualizar el repositorio local con el último commit realizado |
| `git pull origin [nombre rama]` | Traer cambios del repositorio remoto |
| `git remote add origin ssh://git@github.com/[nombre.usuario]/[nombre-repositorio].git` | Añadir un repositorio remoto |
| `git remote set-url origin ssh://git@github.com/[nombre.usuario]/[nombre-repositorio].git` | Fijar la rama origen de un repositorio a SSH |

### Inspección & Comparación

| Comando | Descripción |
| ------- | ----------- |
| `git log` | Ver cambios |
| `git log --summary` | Ver cambios (detallado) |
| `git log --oneline` | Ver cambios (brevemente) |
| `git diff [rama fuente] [rama objetivo]` | Previsualizar cambios antes de fusionar |
