# Practica1Softca
Practica Git y GitHub - Luis Emmanuel Arrieta Bedoya


Crear repositorio

##### 1. Crear un repositorio en vuestro GitHub llamado Practica1Softca

##### 2. Clonar vuestro repositorio en local.
git clone git@github.com:larrieta99/Practica1Softca.git

##### README
##### 3. Crear (si no lo habéis creado ya) en vuestro repositorio local  un documento README.md.


##### Commit inicial
##### 4. Añadir al README.md los comandos utilizados hasta ahora y hacer un commit inicial con el mensaje commit inicial.
git add .
git commit -m "Commit Inicial"

##### Push inicial
##### 5. Subir los cambios al repositorio remoto.
git  pull origin master
git push origin master


##### Ignorar archivos
##### 6. Crear en el repositorio local un fichero llamado privado.txt.
touch privado.txt
##### 7. Crear en el repositorio local una carpeta llamada privada.
mkdir privada
##### 8. Realizar los cambios oportunos para que tanto el archivo como la carpeta sea ignorada por git.
touch .gitignore
code .gitignore
> Dentro del archivo se agrega lo siguiente:
> privada.txt
> /privada

##### Añadir fichero 1.txt
##### 9. Añadir fichero 1.txt al repositorio local.
touch 1.txt

##### Crear el tag v0.1
##### 10. Crear un tag v0.1.
git tag v0.1

##### Subir el tag v0.1
##### 11. Subir los cambios al repositorio remoto.
git push origin --tags
git add .
git pull origin master
git push origin master
##### Crear una rama v0.2
##### 12.. Crear una rama v0.2.
git branch v0.2
##### 13. Posiciona tu carpeta de trabajo en esta rama.
git checkout v0.2
Añadir fichero 2.txt
##### 14. Añadir un fichero 2.txt en la rama v0.2.
touch 2.txt
##### 15. Subir los cambios al repositorio remoto.
git add .
git commit -m "Se creo rama v0.2 con un fichero 2.txt"
git push origin v0.2
##### 16. Posicionarse en la rama master.
git checkout master
##### Merge directo
##### 17.Hacer un merge de la rama v0.2 en la rama master.
git merge v0.2
##### Merge con conflicto
##### 18. En la rama master poner Hola en el fichero 1.txt y hacer commit.
code 1.txt
> Dentro del archivo se agrega lo siguiente:
> Hola

git add .
git commit -m "Se puso Hola en el archivo 1.txt"

##### 19. Posicionarse en la rama v0.2 y poner Adios en el fichero "1.txt" y hacer commit.
git checkout v0.2
code 1.txt
> Dentro del archivo se agrega lo siguiente:
> Adios

git add .
git commit -m "Se puso Adios en el archivo 1.txt"