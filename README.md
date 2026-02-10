# Guía básica de comandos Git

Una referencia rápida y práctica para aprender y usar **Git** y **GitHub** en tus proyectos.

---

## 🚀 Inicialización
- `git init` &rarr; Inicializa un repositorio en la carpeta actual. 
- `git clone <url>` &rarr; Clona un repositorio remoto en tu computadora.

---

## 📂 Estado y cambios 
- `git status` &rarr; Muestra el estado de los archivos. 
- `git add <archivo>` &rarr; Agrega un archivo al área de preparación. 
- `git add .` &rarr; Agrega todos los archivos modificados. 
- `git commit -m "mensaje"` &rarr; Guarda los cambios en el historial. 
- `git commit -am "mensaje"` &rarr; Agrega y guarda cambios en un solo paso. 
- `git diff` &rarr; Muestra diferencias entre archivos.

---

## 🔄 Sincronización con GitHub 
- `git remote -v` &rarr; Lista los repositorios remotos vinculados. 
- `git push origin main` &rarr; Sube tus cambios a GitHub. 
- `git pull origin main` &rarr; Trae la versión más reciente desde GitHub. 
- `git fetch origin` &rarr; Descarga cambios sin fusionarlos. 
- `git push -u origin main` &rarr; Sube la rama principal y la vincula al remoto.

---

## 🧭 Historial 
- `git log` &rarr; Muestra el historial de commits. 
- `git log --oneline` &rarr; Historial compacto. 
- `git log --graph --oneline --decorate --all` &rarr; Historial visual con ramas. 
- `git show <id-commit>` &rarr; Detalles de un commit específico.

---

## 🌿 Ramas 
- `git branch` &rarr; Lista las ramas. 
- `git branch <nombre>` &rarr; Crea una nueva rama. 
- `git checkout <nombre>` &rarr; Cambia de rama. 
- `git switch <nombre>` &rarr; Alternativa moderna a checkout. 
- `git merge <rama>` &rarr; Fusiona una rama en la actual. 
- `git branch -d <nombre>` &rarr; Elimina una rama local. 
- `git push origin --delete <nombre>` &rarr; Elimina una rama remota. 

---

## 🧹 Deshacer cambios 
- `git restore <archivo>` &rarr; Revierte un archivo al último commit. 
- `git reset --soft HEAD~1` &rarr; Deshace el último commit pero conserva cambios. 
- `git reset --hard HEAD~1` &rarr; Vuelve al commit anterior y borra cambios. 
- `git revert <id-commit>` &rarr; Crea un commit inverso (más seguro en equipo). 
- `git stash` &rarr; Guarda cambios temporales sin hacer commit. 
- `git stash pop` &rarr; Recupera los cambios guardados. 

---

## 🛠 Otros útiles 
- `git diff` &rarr; Muestra diferencias entre archivos. 
- `git rm <archivo>` &rarr; Elimina un archivo del repo. 
- `git mv <archivo> <nuevo-nombre>` &rarr; Renombra o mueve un archivo. 
- `git help <comando>` &rarr; Muestra ayuda sobre un comando específico.

---

## 📌 Flujo típico de trabajo 
```bash 
# Traer cambios recientes 
git pull origin main 

# Ver estado 
git status 

# Agregar archivos 
git add . 

# Guardar cambios 
git commit -m "Descripción clara de cambios" 

# Subir a GitHub 
git push origin main
```

---

## 📋 Tabla rápida de referencia

| Comando                  | Qué hace                                | Ejemplo de uso                          |
|---------------------------|-----------------------------------------|-----------------------------------------|
| `git status`              | Muestra estado actual del repo          | `git status`                            |
| `git add .`               | Agrega todos los archivos               | `git add .`                             |
| `git add <archivo>`       | Agrega un archivo específico            | `git add index.html`                    |
| `git commit -m "msg"`     | Guarda cambios en historial             | `git commit -m "Agregando index.html"`  |
| `git push origin main`    | Sube cambios a GitHub                   | `git push origin main`                  |
| `git pull origin main`    | Trae cambios más recientes              | `git pull origin main`                  |
| `git log --oneline`       | Historial compacto                      | `git log --oneline`                     |
| `git branch <nombre>`     | Crea una nueva rama                     | `git branch feature-login`              |
| `git checkout <nombre>`   | Cambia a otra rama                      | `git checkout feature-login`            |
| `git switch <nombre>`     | Alternativa moderna a checkout          | `git switch feature-login`              |
| `git merge <rama>`        | Fusiona una rama                        | `git merge feature-login`               |
| `git reset --hard HEAD~1` | Borra cambios y vuelve al commit previo | `git reset --hard HEAD~1`               |
| `git revert <id-commit>`  | Crea un commit inverso (más seguro)     | `git revert a1b2c3d`                    |
| `git rm <archivo>`        | Elimina un archivo del repo             | `git rm viejo.txt`                      |
| `git mv <archivo> <nuevo>`| Renombra o mueve un archivo             | `git mv index.html inicio.html`         |
| `git diff`                | Muestra diferencias entre archivos      | `git diff`                              |
| `git remote -v`           | Lista repositorios remotos vinculados   | `git remote -v`                         |
