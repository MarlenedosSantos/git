## Clase 02 - Git desarrollo colaborativo 

## Archivo .gitignore 
Existe un archivo que nos permite ignorar ciertos archivos que queremos que no sean parte de los commits. Se crea generalmente en la carpeta raiz del proyecto. 

```sh 
touch .gitignore
```

## Archivo .gitkeep 
Exite un archivo que nos permite agregar a los commit, las carpetas vacias que git por defecto ignora 

```sh 
touch .gitkeep
```

# Subir nuestro repositorio a la nube 
Nos logueamos en Github y creamos un repositorio de Github. Dejo todo por defecto y si quiero cambio la visibilidad, publico todos pueden acceder y solo yo modifico. Privado. Nadie puede verr a menos que los agregue al repositorio para que lo vea.

## Agregar la url del repositorio remeto a repositorio local

```sh 
git remote add <alias> <url> 
git remote add origin https://github.com/MarlenedosSantos/git.git
```

## Confirmar si tengo un remoto en un repo local

```sh 
git remote 
git remote -v # mas detalle -v:verbose
git remote show origin
```

## Subir la copia completa o parcial del commits del local al remoto 

```sh
git push -u <repositorio-remoto> <rama> 
git push -u origin main # -u -> sincronizar la rama local con la remota. Solo la primera vez se agrega el flag/bandera -u
```
git credential-cache exit
git push -u origin main

## Recuperar el repositorio despues de una catastrofe 
Si tengo una copia del repositorio en el remoto puedo recuperar la informacion en el local.

![clone](_ref/clone.png)

```sh
git clone <url> # me crea una carpeta con el nombre del repositorio en el directorio actual 
git clone <url> ./ # copia el repositorio en la carpeta actual 
git clone http://github.com/ylaurlqueva
```

# RAMAS (Branches)
