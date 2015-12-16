# campusciff

#Clonar repositorio en local
- git clone https://github.com/sergiovazquezfeijoo/campusciff.git

#Crear en el repositorio local un fichero llamado privado.txt.
- touch privado.txt

#Crear en el repositorio local una carpeta llamada privada.
- mkdir privada

#Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git
- Creado el fichero el .gitignore agregandole las lineas: privado.txt y privada

# Crear fichero1.txt
- touch fichero1.txt

#Crear un tag v0.1
- git tag -a v0.1 -m "Tag v0.1"

#Subir los cambios al repositorio remoto
- git add .
- git commit -m "Creando fichero1.txt y .gitignore"
- git push --tag origin master

#Crear una rama v0.2.
- git branch v0.2



#Listar los distintos commits con sus ramas y sus tags.
- git config --global alias.list 'log --oneline --decorate --graph --all'
- git list

#Posiciona tu carpeta de trabajo en esta rama.
- git checkout v0.2

#Añadir un fichero 2.txt en la rama v0.2.
- touch fichero2.txt

#Subir los cambios al reposiorio remoto.
- git add .
- git commit -m "Añadido fichero2.txt"
- git push origin v0.2

# Posicionarse en la rama master
- git checkout master

# Hacer un merge de la rama v0.2 en la rama master.
- git merge v0.2

# En la rama master poner Hola en el fichero 1.txt y hacer commit.
- vim fichero1.txt
- git add .
- git commit -m "fichero1.txt modificado"

# Posicionarse en la rama v0.2 y poner Adios en el fichero "1.txt" y hacer commit.
- git checkout v0.2
- vim fichero1.txt
- git add .
- git commit -m "fichero1.txt modificado en v0.2"

# Posicionarse de nuevo en la rama master y hacer un merge con la rama v0.2
- git checkout master
- git merge v0.2
- vim fichero1.txt
- git add .
- git commit -m "resuelto conflicto en fichero1.txt"

# Listar las ramas con merge y las ramas sin merge.
- git branch --merged
- git branch --no-merged

# Crear un tag v0.2
- git tag -a v0.2 -m "Tag v0.2"

# Borrar la rama v0.2
- git branch -d v0.2

#Crear keys
Sergio
74:f3:59:58:4e:07:12:4b:5a:8f:65:20:30:18:89:46
Added on Dec 15, 2015 — Never used

#Tabla compañeros de clase
| Patricia Iglesias | <https://github.com/Pimateos/> |
| Ulises Ojeda | <https://github.com/ulisesojeda/> |
| David Pacheco | <https://github.com/davpacheco/> |
| Sergio Torres | <https://github.com/sergiotorrespalomino/> |




