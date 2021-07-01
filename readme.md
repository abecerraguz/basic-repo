# VER PASOS DE SUBIDA A REPO

```
CONFIGURAR GIT + GITHUB

1/   git config --list 

2/   Para asignar el usuario y el correo
     git config --global user.name "XXXXXXXXXXX"
     git config --global user.email "XXXXXXXXXX"

3/   Ir a la URL https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
     Seguir las Instrucciones:
     Antes del paso uno de la URL Escribir en el terminal, Esto nos mostrara el Listado oculto de la Carpeta SSH, se listara
     -   ls -al ~/.ssh
     -   ssh-keygen -t rsa -b 4096 -C "alejandro.becerra@publimetro.cl"
     -   Luego te pregunta donde dejar las llaves, sólo hacer Enter

4/  Agregar y Probar mi clave SSH
    - Agregar la clave privada a nuestro ssh-agent
    - eval "$(ssh-agent -s)"      
    - ssh-add ~/.ssh/id_rsa

      Para copiar la clave en Mac
    - pbcopy < ~/.ssh/id_rsa.pub

      Para copiar la clave en Window
    - $ clip < ~/.ssh/id_ed25519.pub


    Para copiar la clave en Linux
    - sudo apt install xclip (Instala una aplicacion para copiar), Luego se debe escribir
      xclip -sel clip < ~/.ssh/id_rsa.pub
    - Para saber si se conecto con GitHub
      ssh -T git@github.com

      Paso Uno
      llegas a la carpeta que vas iniciar con git ejemplo git cd Desktop/mi_carpeta, luego 
      
      git init
      git add .
      git commit -m "Mi pimer commit"

      Paso Dos
      Ir al HTML hacer un cambio, luego nuevamente
      git add .
      git commit -m "Segundo commit"

      Paso Tres para ver el estado de los commit
      git status
      git log

	 Eliminar Branch
	 git branch -d gh-pages

	 Eliminar git
	 rm -rf .git
```

