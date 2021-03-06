# Interactuar con este repo.
## La primera vez.
Abrir Git Bash en la carpeta que va a contener el código y ejecutar:

0. Si nunca usaron Git en la computadora, primero hay que configurar usuario de Git:
```
git config --global user.email "you@example.com"
```
1. Primero hay que clonar el repositorio master:
```
git clone https://github.com/manuperotti/dh_ds_grupo2_desafio1.git
```
Copiar la notebook al directorio del repositorio, que debería llamarse **dh_ds_grupo2_desafio1**. 
Parados dentro del repositorio, ejecutar por bash:

2. Después hay que agregar el directorio completo sobre el que están parados:
```
git add .
```
3. Se realiza un commit inicial para que Git pueda detectar los cambios entre el origen y el master:
```
git commit -m "Descripción del cambio"
```
4. Por último, se ejecuta este comando para subir los cambios al master:
```
git push -u origin master
```
## Por cada vez que lo actualizan.
Abrir el Git Bash en el repositorio dh_ds_grupo2_desafio1 y ejecutar los comandos listados.
1. Primero hay que ver si hay cambios en el master. Con este comando se actualiza el repositorio local:
```
git pull https://github.com/manuperotti/dh_ds_grupo2_desafio1.git
```
2. A continuación, se hace un commit para que Git pueda detectar los cambios entre el origen y el master:
```
git commit -m "Nombre cambios en la notebook"
```
A veces da error el commit diciendo que no hay cambios. Si pasa esto, ejecutar el comando para agregar a mano los archivos que hayan cambiado:
```
git add [archivo]
```
3. Por último, se ejecuta este comando para subir los cambios al master:
```
git push -u origin master
```
## En caso de errores, para forzar el download.

Estos comandos actualizan todos los archivos del master en el local:
```
git fetch --all
git reset --hard origin/master
```
