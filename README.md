# Practica1Softca
Practica Git y GitHub - Luis Emmanuel Arrieta Bedoya


Crear repositorio

#####1. Crear un repositorio en vuestro GitHub llamado Practica1Softca

#####2. Clonar vuestro repositorio en local.
git clone git@github.com:larrieta99/Practica1Softca.git

#####README
#####3. Crear (si no lo habéis creado ya) en vuestro repositorio local  un documento README.md.


#####Commit inicial
#####4. Añadir al README.md los comandos utilizados hasta ahora y hacer un commit inicial con el mensaje commit inicial.
git add .
git commit -m "Commit Inicial"

#####Push inicial
#####5. Subir los cambios al repositorio remoto.
git  pull origin master
git push origin master


#####Ignorar archivos
#####6. Crear en el repositorio local un fichero llamado privado.txt.
touch privado.txt
#####7. Crear en el repositorio local una carpeta llamada privada.
mkdir privada
#####8. Realizar los cambios oportunos para que tanto el archivo como la carpeta sea ignorada por git.
touch .gitignore
code .gitignore
> Dentro del archivo se agrega lo siguiente:
> privada.txt
> /privada

#####Añadir fichero 1.txt
#####9. Añadir fichero 1.txt al repositorio local.
touch 1.txt

#####Crear el tag v0.1
#####10. Crear un tag v0.1.
git tag v0.1

#####Subir el tag v0.1
#####11. Subir los cambios al repositorio remoto.
git push origin --tags
git add .
git commit -am "Se añaden todos los cambios"
git pull origin master
git push origin master