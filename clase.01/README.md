#Clase 01 - Git Desarrollo Colaborativo 

## Configuracion inicial 

### Configurando nombre y correo 

```sh
git config --global user.name "MarlenedosSantos"
git config --global user.email "marlene.dossantos97@gmail.com" 
```

### Configuración del editor 

```sh 
git config --get-regexp editor
```

### Por defecto rama main 

```sh 
git config --global init.defaultBranch main 
```

# Inicializando un repositorio de GIT 

```sh 
git init
```

### Para cambiar el repo de master a main o al revés

```sh
rm -rf .git
git config --global init.defaultBranch main
```

# Controlar el status de los archivos del proyecto
```sh
git status
```
## Areas posibles en las que pueden estar los archivos
* Working Directory (Directo de trabajo) donde van agregando, borrando al archivo el desarrolllo
* Staging Area (Area de control de cambios) Se agregan los archivos para darle seguimiento y posteriormente sacarles una foto (commit)
* Local Repo (Area de validación de cambios, donde se registran las modificaciones realizadas) Donde van a estar todas las fotos (commit) que vaya sacando.

## Estados de los archivos
* Untracked (Sin seguimiento) => archivos que no se agregaron al index/stage y por consecuente no se les da seguimiento.
* Staged => Archivos que fueron agregados al index/stage area y cuyos cambios van a ser incorporados al repositorio
* Unmodified => Archivos que se cuentran en en el respositorio y no fueron modificado (Con respecto al repositorio)
* Modified => Archivos que se encuentro en el repositorio pero difieren con lo que se encuentra actualmente en el directorio trabajo (Working directory)

## Agregar a la zona de Staging (marcar el archivo o archivos para que formen parte del commit)

```sh 
git add <nombre-archivo>
git add clase.01/README.md
git add . #Agrega todo a la zona de confirmacion (Staging area)
```
# Quitar de la zona de Staging 

```sh
git restore --staged <nombre-archiv>
git restore --staged clase.01/README.md
```

# Hacer un commit (backup, snapshot)

```sh
git commit -m "mensaje descriptivo"
git commit # Me abre el editor para yo poder escribir el titulo y el cuerpo de la descripcion. Crtl + O -> Crtl + X
```

## Ver la diferencia entre el working directory y el local repo 

```sh
git diff 
git diff <nombre-archivo>
git diff clase.01/README.md # Q para salir del diff
```

