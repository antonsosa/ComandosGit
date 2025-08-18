# ComandosGit
En este archivo voy recopilando los comandos que más se utilizan en Git
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