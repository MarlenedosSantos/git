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

### ???????

```sh
git status
``` 

## Areas posibles en las que pueden estar los archivos

*
*
*

## Estados de los archivos 