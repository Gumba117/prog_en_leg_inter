# Practica 8
Dante Misael Osornio G. CDMX2592
## ¿Cómo se inicializa un repositorio en Git?
Usas el comando Init en la terminal git bash:
```bash
$ git init
```
## ¿Cómo creas un repositorio en GitHub?
En github le das al boton que dice "Create a new repository", sigues los pasos que te da la pagina de github.

## ¿Cómo vinculas un repositorio local de Git con uno remoto en GitHub?

Con el git iniciado, usas el comando remote add origin para vincularlo con el git en la nube usas el link de github y le pones .git al final 

```bash
$ git remote add https://github.com/Gumba117/prog_en_leg_inter.git
```

## ¿Cuál es el flujo básico de trabajo en Git y GitHub?

Se empieza el repositorio, creas el gitignore, eliges una licencia y añades un readme.
Una ves que ya se tiene el repositorio 
Se usa add .  para añadir los archivos nuevo o modificados a un commit, despues se usa commit y se le pone un nombre identificador al commit.
Finalmente con el comando push lo subes a la nube
Si ya tienes el repositorio en la nube o algien mas trabajo en el se usa fetch para descargar los archivos y despues pull para integrarlos a el local.

```bash
$ git add .
$ git commit -m "Nombre del commit"
$ git push -u origin main
$ git fetch
$ git pull 
```

## ¿Para qué sirve el archivo .gitignore?

Sirve para evitar que ciertos archivos o tipos de archivos no entren en git, osea que git los ignora es por eso que se llama gitIGNORE

## ¿Cuál es el propósito de una rama?

Las ramas son un entorno de pruebas seguro para desarrollar codigo experimental sin que dañe el codigo principal. Se pueden hacer con el comando git branch y el nombre de la branch

```bash
$ git branch rama_1
```

## ¿Qué es una fusión?

Es cuando 2 ramas se unen. Se puede hacer con el comando git merge y la rama a la que te quieres unir, todo esto desde la rama que quieres que se una.

## Explica los diferentes tipos de fusión que existen.

Existe la fusion sin porblemas y la fusion con problemas
En la fusion sin problemas ningun archivo tiene conflicto entre las 2 branches.

En la fusion con problemas uno o mas archivos tienen conflictos generalmente por que son distintos internamente pero se llaman igual, en este caso se tiene que elegir cual de los 2 archivos se queda en el repositorio manualmente.

## ¿Cómo puedes ver el historial de tu repositorio?

En github puedes ver los commits que se han hecho, por otro lado se puede usar el comando git log para ver los cambios, pero tambien se puede usar con el comando oneline para que se vea mas bonito y sea mas facil de leer.

```bash
$ git log
$ git log --oneline
```

## ¿Cuál es el propósito de una etiqueta?

Las etiquetas son versiones estables de un repositorio, tienen la nomenclatura V1.0.0
Que es V de version , 1 numero de version, 0 la actualizacion y 0 el arreglo de bugs.
Osea si hay una tag 2.17.3, es la version 2 la actualizacion 17 y hay 3 bugfixes.