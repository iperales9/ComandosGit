# 🚀 Guía de Comandos Git 🚀

## 1. Configurar credenciales globales
```bash
git config --global user.name "Ivan"
git config --global user.email "ivan@example.com"
git config --global alias."NombreDelAlias" "ComandoAsociado"
```
📌 **Los alias pueden ayudarte a abreviar comandos largos.**  

---

## 2. Inicializar y gestionar el repositorio
```bash
git init  # Inicializa un repositorio Git  
```

---

## 3. Añadir y confirmar cambios
```bash
git add .   # Agrega todos los archivos modificados al área de preparación  
git commit -m "Descripción del commit"  # Guarda los cambios en la rama actual  
```

---

## 4. Historial de cambios
```bash
git log --oneline  # Muestra un historial breve de commits  
git reflog  # Muestra todos los cambios hechos en el repositorio  
git diff  # Muestra las diferencias del último commit  
```

---

## 5. Gestión de ramas
```bash
git branch "nombre-de-la-rama"  # Crear una nueva rama  
git branch -d "nombre-de-la-rama"  # Eliminar una rama  
git branch -m "nuevo-nombre"  # Renombrar la rama actual  
git checkout "nombre-de-la-rama"  # Cambiar a otra rama (obsoleto en versiones recientes)  
git switch "nombre-de-la-rama"  # Alternativa moderna a checkout  
```

---

## 6. Fusionar ramas
```bash
git merge "nombre-de-la-rama"  # Fusionar una rama con la actual (normalmente main)    
```
📌 **Antes de hacer merge, asegúrate de estar en la rama principal y que no haya conflictos.**

---

## 7. Clonar repositorio
```bash
git clone "URL-del-repositorio" .  # Clonar en el directorio actual  
```

---

## 8. Subir y descargar cambios
```bash
git push origin "nombre-de-la-rama"  # Subir commits al repositorio remoto  
git pull  # Descargar los últimos cambios del repositorio remoto  
```

---

## 9. Gestión de commits
```bash
git reset --hard "ID-del-commit"  # ⚠️ Restablece el historial de commits (¡Cuidado!)  
git stash  # Guarda temporalmente los cambios sin hacer commit  
git stash list  # Ver stashes guardados  
git stash pop  # Recuperar cambios del stash  
git stash drop  # Eliminar un stash  
```

---

## 10. Etiquetas en commits
```bash
git tag "nombre-de-la-etiqueta"  # Crear una etiqueta en un commit importante  
```

---

## 11. GitFlow
```bash
git flow init # Inicializa el repositorio con git flow  
git flow "feature,release,hotfix,support,version" start "Nombre de la rama" # Inicia la rama que queramos crear  
git flow "feature,release,hotfix,support,version" finish "Nombre de la rama" # Finalizamos la rama y la junta con develop  
```

## 12. Cherry-pick y rebase
### ⚠️ Evitar utilizarlos si no es precisamente necesario ⚠️
```bash
git cherry-pick "ID-del-commit"  # Aplicar un commit específico en otra rama  
git cherry-pick --continue  # Continuar el proceso de cherry-pick después de resolver conflictos  
git rebase "nombre-de-la-rama"  # Reaplicar commits sobre otra base para mantener un historial más limpio  
```


---

## 📈 Guía diseñada para ayudarte a manejar Git de manera eficiente. 🚀
