# Este archivo es para saber usar git y GitHub
## Codigos de GitHub que me pueden servir 
### Comandos mas usados
- `git init` 
### Para volver a usar mi repositorio
- `cd ruta/del/repositorio`: Accedemos al lugar en donde esta el repositorio dentro de nuestro escritorio
- `git status`: Este comando te dice si estas en un main o en otra rama
- `git pull origin main`: Para traer la version mas reciente
### Para subir los archivos de manera local por medio de visual studio
- `git status`: Para ver si hay cambios por realizar
- `git add .`: Para subir todos los archivos o para archivo especifico usar `git add nombre_archivo.ext`
- `git commit -m "Agregando nuevos archivos"`: Esto guarda los cambios en un historial local
- `git push` o `git push origin main`: Para poder subir los archivos
Ejemplo de como quedaria:
```
git status
git add index.html
git commit -m "Creando archivo index.html"
git push origin main
```
Tips utiles
- Si ya habías hecho cambios y quieres subir todo de golpe:
```
git add .
git commit -m "Actualización general"
git push origin main
```
- Si te pide usuario/contraseña, asegúrate de tener configurado el SSH key o el token de acceso personal en GitHub.
-Puedes confirmar que se subió entrando al repositorio en GitHub y revisando los archivos.
### Para ver el historial y que commit usar
- `git log`: Para poder ver el historial de actualizaciones
    - `q` Para salir del historial de actualizaciones
Algunos atajos de git log son:
- Espacio &rarr; avanza una pagina
- Enter &rarr; avanza una linea
- b &rarr; retrocede una pagina
- q &rarr; salir del log
### Comandos basicos
Inspeccion y estado
- `git status` &rarr; Muestra el estado actual de tu repo (archivos modificados, pendientes de commit, etc.).
- `git diff` &rarr; Muestra las diferencias entre tu carpeta y el último commit.
- `git log --oneline` &rarr; Historial compacto de commits.
- `git show <id-commit>` &rarr; Muestra detalles de un commit específico.
Manejo de archivos
- `git add archivo` &rarr; Agrega un archivo al staging.
- `git rm archivo` &rarr; Elimina un archivo del repo y lo marca para commit.
- `git mv archivo-nuevo archivo-viejo` &rarr; Renombra o mueve un archivo.
