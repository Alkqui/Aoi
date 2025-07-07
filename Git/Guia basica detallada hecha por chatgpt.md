# Guía rápida y detallada de Git con ejemplos sencillos

## 🔷 Inicializar repositorio

Crea un repositorio vacío en la carpeta actual.

```
git init
```

📌 **Ejemplo:**

```
cd mi-proyecto
git init
```

Resultado: Se crea una carpeta oculta `.git` donde Git guarda su información.

---

## 🔷 Ver estado

Muestra los archivos modificados y pendientes de guardar (staging).

```
git status
```

📌 **Ejemplo:**

```
git status
```

Resultado: "modified: archivo.txt"

---

## 🔷 Ver historial de commits

Muestra los commits realizados.

```
git log
```

📌 Compacto:

```
git log --oneline
```

---

## 📝 Trabajar con cambios

### Añadir archivos al staging

```
git add archivo.txt
```

O todos los archivos:

```
git add .
```

### Quitar archivo del staging

```
git restore --staged archivo.txt
```

### Descartar cambios en archivo

```
git restore archivo.txt
```

---

## 💾 Guardar cambios

### Crear un commit

```
git commit -m "Mensaje descriptivo"
```

### Añadir y commitear en un solo paso

```
git commit -am "Mensaje"
```

📌 Solo funciona si los archivos ya estaban bajo seguimiento.

---

## 🌲 Ramas

### Ver ramas

```
git branch
```

### Crear nueva rama

```
git branch nueva-rama
```

### Cambiar de rama

```
git switch nombre-rama
```

### Crear y cambiar a nueva rama

```
git switch -c nueva-rama
```

---

## 🔄 Fusionar ramas

### Fusionar otra rama en la actual

```
git merge otra-rama
```

### Rebase (avanzado)

```
git rebase otra-rama
```

---

## 🔍 Ver diferencias

### Ver cambios no agregados

```
git diff
```

### Ver cambios en staging

```
git diff --staged
```

### Ver cambios entre ramas

```
git diff main..feature
```

---

## 🌐 Trabajar con repositorios remotos

### Conectar a remoto

```
git remote add origin URL
```

### Ver remotos

```
git remote -v
```

### Subir cambios

```
git push -u origin main
```

Luego solo:

```
git push
```

### Traer cambios

```
git pull
```

### Clonar repositorio

```
git clone URL
```

---

## ✨ Comandos modernos útiles

✅ Cambiar de rama (más claro que `checkout`):

```
git switch nombre-rama
```

✅ Crear y cambiar a nueva rama:

```
git switch -c nueva-rama
```

✅ Restaurar archivo (descartar cambios locales):

```
git restore archivo.txt
```

✅ Quitar archivo del staging:

```
git restore --staged archivo.txt
```

---

## 🚀 Flujo básico recomendado

1️⃣ Inicializa repo:

```
git init
```

2️⃣ Haz cambios y revisa:

```
git status
```

3️⃣ Añade al staging:

```
git add .
```

4️⃣ Crea commit:

```
git commit -m "Primera versión"
```

5️⃣ Conecta a remoto:

```
git remote add origin URL
```

6️⃣ Sube:

```
git push -u origin main
```

7️⃣ Sigue trabajando en ramas y `commit` + `push` regularmente.