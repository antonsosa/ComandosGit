# ComandosGit
En este archivo voy recopilando los comandos que más se utilizan en Git
---
# Antes que nada a instalar Git
  Ve al sitio web oficial de Git: https://git-scm.com/
  
  -Información de licencia: Haz clic en Next.
  
  -Seleccionar componentes: Deja las opciones por defecto marcadas. Es importante que Git Bash y Git GUI estén seleccionados. Git Bash es una terminal para ejecutar comandos de Git. Haz clic en Next.
  
  -Seleccionar carpeta de instalación: Generalmente se recomienda dejar la ruta por defecto. Haz clic en Next.
  
  -Seleccionar el editor por defecto para Git: Aquí puedes elegir tu editor de código preferido, como Visual Studio Code. Asegúrate de que VS Code esté instalado previamente.
  
  -Ajustar el nombre de la rama inicial: Deja la opción por defecto que dice Let Git decide (Dejar que Git decida). Esto usará la rama main, que es el estándar actual. Haz clic en Next.
  
  -Ajustar tu PATH: Elige la opción Git from the command line and also from 3rd-party software. Esta es la opción más recomendada, ya que te permite usar Git desde cualquier terminal, incluyendo la de VS Code.
  
  -Usar la biblioteca de cifrado SSL/TLS: Deja la opción por defecto Use the OpenSSL library.
  
  -Configurar las terminaciones de línea de checkout: Usa la opción por defecto Checkout Windows-style, commit Unix-style line endings.
  
  -Configurar el emulador de terminal para Git Bash: Deja la opción por defecto Use MinTTY (the default terminal of MSYS2).
  
  -Opciones adicionales: Deja las opciones por defecto activadas. Haz clic en Install.

Una vez que la instalación termine, haz clic en Finish.

---

## 1. Configuración inicial de Git
Ver la version de Git
```bash
git -v
```
Configura tu nombre y correo abriendo GitBash o en Terminal/Bash en VSCode:
```bash
git config --global user.name "Tu Nombre" 
```
```bash
git config --global user.email "tuemail@example.com"
```

Verifica la configuración:
```bash
git config --list
```

## 2. Clonar un repositorio existente
Copia el repositorio de GitHub a tu máquina:
```bash
git clone https://github.com/usuario/repositorio.git
```

## 3. Estado del proyecto
Muestra los cambios realizados:
```bash
git status
```

## 4. Añadir archivos al staging
Agrega todos los archivos modificados:
```bash
git add .
```
O agrega un archivo específico:
```bash
git add archivo.txt
```

## 5. Crear un commit
Guarda los cambios con un mensaje:
```bash
git commit -m "Mensaje descriptivo del cambio"
```

## 6. Subir cambios a GitHub
Envía tus commits al repositorio remoto:
```bash
git push origin main
```

## 7. Descargar cambios del remoto
Actualiza tu proyecto con los últimos cambios del repositorio:
```bash
git pull origin main
```


## 8. Ramas (Branches)
Crear una nueva rama:
```bash
git checkout -b nombre-rama
```
Cambiar a una rama existente:
```bash
git checkout nombre-rama
```

## 9. Comandos útiles extra
Ver historial de commits:
```bash
git log --oneline --graph --decorate
```
Eliminar un archivo del staging:
```bash
git reset archivo.txt
```
