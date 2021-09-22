# GIT
    Es un control de versionamientos de archivos

## CREAR CUENTA EN GITHUB

### Configurar credenciales
    Debemos indicarle al sistema qué usuario se conectará con los repositorios de la nube de GitHub

#### git config --global user.name "tu Nombre de usuario de Git"
#### git config -- global user.email "tu correo"

#### git init
    Es para inicializar un repositorio desde de la consola. Esto indicará que los archivos que estén en la carpeta se podrán subir dinámicamente a la nube.

#### git status 
    Este comando nos permite evaluar si hay nuevos archivos o cambios en el repositorio que no hayan sido guardados o anexados

#### git add . 
    Este comando nos permite añadir los archivos y/o carpetas a una fase llamada staging, preparando los  archivos para su posterior carga al repositorio de la nube	
    El punto ( . ) nos indica que se anexarán todos los archivos que tengamos.
    Otra indicación es git add -A que cumple con la misma función.
    Si deseamos anexar un archivo en específio, indicamos el comando git add nombreArchivo

### "git rm --cached <file>..."
    Para remover archivo añadido

#### git commit -m 
    Con este comando indicamos un comentario que sea referente a los archivos que acabamos de anexar.
	Siempre debemos indicarle el comentario por medio de las comillas. Este comentario debe ser claro, conciso con un límite de un tweet (300 caracteres)
	Ejemplo:
        git commit -m "Esto es un ejemplo de comentario"

### git branch -M main
    Aqui le indicamos en cual rama vamos a enviar nuestro commit

#### git remote add origin
    Debemos enlazar nuestro repositorio local con nuestro repositorio en la nube a través de la url
	Ejemplo:
		git remote add origin https://github.com/usuarioPepe/repositorioPrueba

#### git push -u origin main
    Este comando nos permite subir nuestro archivos anexados en git add a nuestro repositorio enlazado en git remote add origin.

### Notas
Tener en cuenta: Estos son los pasos cuando es cremos nuestro un primer repositorio, es decir, un nuevo proyecto.
Si éste ya existe, no tenemos la necesidad de iniciar nuevamente el repositorio local ni enlazarlo con el repo de la nube
Haremos los siguientes pasos:
    git add .
	git status
	git commit -m "NO OLVIDES EL COMENTARIO AQUI"
	git push origin main

De esta forma hemos actualizado nuestro repositorio de la nube.

-------------------------------------------------------------------------------------------

### Descargar o clonar repositorio

En este caso que no tengamos el proyecto en el cual estamos trabajando, descargaremos el repo de la nube

#### git clone
    Clona el repositorio remoto (de la nube) a nuestro repositorio local (nuestro pc)
    Este comando necesita la url del repo que necesitamos clonar
    Ejemplo: 
	    git clone https://github.com/usuarioPepe/repositorioPrueba

#### git pull
    Se encarga de actualizar el repositorio a la última versión existente en la rama principal (rama main)
	Ejemplo:
		git pull origin master

SOY UN TEXTO NUEVO version 2
