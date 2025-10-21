## Guía de GIT

1 - Inicializar Git en un proyecto:
    -   git init

2 - Registrar ficheros nuevos 
    -   git add <Nombre del Fichero>
    -   git add . (el punto hacer referencia a todos los archivos nuevos)

3 - Commit (Necesario para que subirlo, pide un mensaje)
    -   git commit "mensaje de los que se ha heco"

4 - Para movernos en el tiempo a un commit 
    -   git checkout <numero de referencia del commit>
    -   git status (visualizamos el estado)

5 - Para volver acoplarnos a la rama dond estabamos 
    -   git checkout <nombre de la rama>

6 - Para crear una rama nueva 
    -   git checkout -b <nombre de la rama nueva>

7 - Para movernos de ramas 
    -   git checkout <nombre de la rama>

8 - Para traer los cambios de una rama en la que hemos estado trabajando, nos situamos en la rama en la que queremos traer los cambios en este caso sería la rama main, queremos traer los cambios que hemos hecho en la rama dev.
    -   git merge <nombre de la rama>

10 - Autenticar el git mediante comando git hub cli
    - Instalamos el gh (vamos a la web y nos da el comando)
    - Debemos estar registrados en github
    - Ejecutamos comando en la consolo gh auth login
    - Seguimos lo pasos y damos protocolo https
    - Decimos através de el browser y nos dará un código y autorizamos
    - Creamos el nuevo repositorio

11 - Ligar un repositorio local con nuestro repositorio remoto
    - git remote add origin <URL_repositorio_remoto>
    - Subimos código con: git push -u origin  main
    - git pull - Nos trae los cambios que haya en el remoto
    - git fetch - No dice los cambios que hay pero no los actualiza

12 - Fusionar una rama con PULL REQUEST
    - se hace desde el repositorio remoto
    - luego nos pedirá hacer un merge 

13 - Estado de git
    - git status - Nos dice el estado 
    - git log - Lleva un registro de lo que hemos realizado

14 - Conflictos en git
    - realizamos un merge de la rama con el comando git merge <nombre rama>
    - si tenemos conflicto lo resolvemos 
    - realizamos un commit (sin mensaje)
    - por último realizamos un git merge <nombre de la rama>

17 - Otras utilidades de Git
    - git stash - Guarda los cambios de forma temporal, nos permite cambiar de rama para resolver algo en otra rama. (esto se queda guardado y podemos movernos)
    - para devolver los cambios que hemos guardado realizamos el comando "git stash apply"
    pero este no borra el stash. 
    - Si queremos que lo borre del stash realizamos el sigueinte comando "git stash pop"

18 - Estados de un fichero en git 
    - Untracked -> Git no tiene registro sobre el fichero
    - Modified -> Git conoce el fichero y detecta que tiene cambios con respecto al último commit
    - Staged -> El fichero con cambios está listo para añadirse a un commit
    - Commited -> El fichero con cambios ha sido guardado dentro de una revisión

19 -  GIT RESET 
    - Sirve para sacar un fichero que no queremos hacer commit, comando git reset HEAD <NOMBRE DEL FICHERO>

20 - GIT REVERT
    - Deshace los cambios realizados por un commit anterior creando un commit completamente nuevo, no altera el historial de commits

21 - GIT RM
    - Con esto le decimos a git que deje de seguir los cambios de un fichero, eleminandolo de manera efectiva de su índice de trabajo.
    Hay varias opciones:
        - -cached -> mantiene el archivo en la working directory y como untracked.
        - -recursive.





