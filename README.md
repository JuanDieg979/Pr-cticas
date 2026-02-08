# Guía básica de comandos Git

## 🚀 Inicialización
- `git init` &rarr; Inicializa un repositorio en la carpeta actual. 
- `git clone <url>` &rarr; Clona un repositorio remoto en tu computadora.

## 📂 Estado y cambios
- `git status` &rarr; Muestra el estado de los archivos. 
- `git add <archivo>` &rarr; Agrega un archivo al área de preparación.
- `git add .` &rarr; Agrega todos los archivos modificados. 
- `git commit -m "mensaje"` &rarr; Guarda los cambios en el historial.

## 🔄 Sincronización con GitHub 
- `git remote -v` &rarr; Lista los repositorios remotos vinculados. 
- `git push origin main` &rarr; Sube tus cambios a GitHub. 
- `git pull origin main` &rarr; Trae la versión más reciente desde GitHub. 
- `git fetch origin` &rarr; Descarga cambios sin fusionarlos.

## 🧭 Historial 
- `git log` &rarr; Muestra el historial de commits. 
- `git log --oneline` &rarr; Historial compacto. 
- `git show <id-commit>` &rarr; Detalles de un commit específico.

## 🌿 Ramas 
- `git branch` &rarr; Lista las ramas. 
- `git branch <nombre>` &rarr; Crea una nueva rama. 
- `git checkout <nombre>` &rarr; Cambia de rama. 
- `git switch <nombre>` &rarr; Alternativa moderna a checkout. 
- `git merge <rama>` &rarr; Fusiona una rama en la actual.

## 🧹 Deshacer cambios 
- `git restore <archivo>` &rarr; Revierte un archivo al último commit. 
- `git reset --soft HEAD~1` &rarr; Deshace el último commit pero conserva cambios. 
- `git reset --hard HEAD~1` &rarr; Vuelve al commit anterior y borra cambios. 
- `git revert <id-commit>` &rarr; Crea un commit inverso (más seguro en equipo).