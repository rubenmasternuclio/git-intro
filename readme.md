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



