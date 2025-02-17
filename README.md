# Anotaciones Libro

<h1>Anotaciones Libro</h1>

<h2>...</h2>
<h2>Git y gitHUb: reposistorio, commit y versiones</h2>
<p>Dentro de los comando más comunenes se tienen:</p>
<ol start="3">>
  <li>git clone https://github.com/Lu1sMig/sistema-de-registro..git</li>
<dl>
  <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~<br />
$ git config --global user.mail lmcavero.a@gmail.com
</dt>
  <dd>se valida con el correo del usuario</dd>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~<br />
$ git config --global user.name "Lu1sM1g"
  </dt>
  <dt>
    SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~<br />
$ git config --list<br/</dt>
        <dd>diff.astextplain.textconv=astextplain<br />
        filter.lfs.clean=git-lfs clean -- %f<br />
        filter.lfs.smudge=git-lfs smudge -- %f<br />
        filter.lfs.process=git-lfs filter-process<br/>
        filter.lfs.required=true<br/>
        http.sslbackend=openssl<br/>
        http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt<br/>
        core.autocrlf=true<br/>
        core.fscache=true<br/>
        core.symlinks=false<br/>
        pull.rebase=false<br/>
        credential.helper=manager<br/>
        credential.https://dev.azure.com.usehttppath=true<br/>
        init.defaultbranch=master<br/>
        user.mail=lmcavero.a@gmail.com<br/>
        user.email=luis.cavero3@unmsm.edu.pe<br/>
        user.name=Lu1sM1g<br/>
        filter.lfs.clean=git-lfs clean -- %f<br/>
        filter.lfs.smudge=git-lfs smudge -- %f<br/>
        filter.lfs.process=git-lfs filter-process<br/>
        filter.lfs.required=true<br/>
 </dd>
</dt>
<dt>$ git log</dt>
<dd>historial de conecciones al repositorio</dd>
<dt>$ git log --oneline</dt>
<dd>historial por conectar a git</dd>
<dt>$ git log -p</dt>
<dd>Historial detallado de cambio del repositorio</dd>
<dt>git log --since=1.month-ago --until=1.day.ago</dt>
<dd>Historial de cambios en un lapso de tiempo</dd>
<dt>$ git log --pretty="format:%h %s"</dt>
<dd>historial con formato.</dd>

<dt>Git mostrará el nombre de la rama principal (rama) que está en uso, que generalmente se llama master.</dt>
<dd><prep>*Nota: Para garantizar la compatibilidad futura, se recomienda actualizar el nombre de la rama de master a principal con el siguiente comando:<br/>
$ git branch -M main</prep></dd>
  
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br />$ git status</dt>
<dd>On branch main<br/> Your branch is up to date with 'origin/main'.<br/>Untracked files:<br/>  (use "git add <file>..." to include in what will be committed)<br/>contacto.html<br/>
nothing added to commit but untracked files present (use "git add" to track)
</dd>

<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>$ git add .</dt>
<dd></dd>

<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>
$ git commit -m "archivo contacto"</dt>
<dd> [main 83a55b0] archivo contacto <br\> 1 file changed, 12 insertions(+) <br/> create mode 100644 contacto.html</dd>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>$ git push</dt>
<dd>info: please complete authentication in your browser...<br/>
Enumerating objects: 4, done.<br/>
Counting objects: 100% (4/4), done.<br/>
Delta compression using up to 8 threads<br/>
Compressing objects: 100% (3/3), done.<br/>
Writing objects: 100% (3/3), 540 bytes | 540.00 KiB/s, done.<br/>
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)<br/>
To https://github.com/Lu1sMig/sistema-de-registro.git<br/>
   0569fe7..83a55b0  main -> main<br/>
</dd>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>$ git status</dt>
<dd>On branch main<br/>Your branch is up to date with 'origin/main'.<br/>nothing to commit, working tree clean</dd>
</dl>
  
<li>Ramificaciones y merge
  <dl>
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br />$ git branch<br/></dt>
    <dd>* main</dd>
                     
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>$ git checkout -b desarrollo</dt>
    <dd>Switched to a new branch 'desarrollo'</dd>
    
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)<br/>$ git switch main</dt>
    <dd>Switched to branch 'main'<br/>Your branch is up to date with 'origin/main'.</dd>
    
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>$ git branch</dt>
    <dd>desarrollo<br/>* main</dd>

    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)<br/>
    $ git add .</dt>
    
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)<br/>
    $ git commit -m "agregando instructor datos"</dt>
    <dd><prep>[desarrollo 6bc3db7] agregando instructor datos
       1 file changed, 1 insertion(+)</prep></dd>
       
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)<br/>
    $ git push</dt>
    <dd><prep>fatal: The current branch desarrollo has no upstream branch.
    To push the current branch and set the remote as upstream, use
        git push --set-upstream origin desarrollo
       To have this happen automatically for branches without a tracking
    upstream, see 'push.autoSetupRemote' in 'git help config'.
    </prep></dd>
    
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)<br />
    $ git push origin desarroll</dt>
    <dd><prep>
    error: src refspec desarroll does not match any
    error: failed to push some refs to 'https://github.com/Lu1sMig/sistema-de-registro.git'</prep></dd>

    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)<br/>
    $ git push origin desarrollo</dt>
    <dd><prep>
    Enumerating objects: 30, done.
    Counting objects: 100% (30/30), done.
    Delta compression using up to 8 threads
    Compressing objects: 100% (24/24), done.
    Writing objects: 100% (30/30), 7.50 KiB | 3.75 MiB/s, done.
    Total 30 (delta 9), reused 16 (delta 3), pack-reused 0 (from 0)
    remote: Resolving deltas: 100% (9/9), done.
    remote:
    remote: Create a pull request for 'desarrollo' on GitHub by visiting:
    remote:      https://github.com/Lu1sMig/sistema-de-registro/pull/new/desarrollo
    remote:
    To https://github.com/Lu1sMig/sistema-de-registro.git
     * [new branch]      desarrollo -> desarrollo</prep></dd>
     
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main) <br/>$ git init</dt>
    <dd>Reinitialized existing Git repository in C:/Users/SOPORTE/Documents/GitHub/sistema-de-registro/.git/<br />
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br />$ git status</dt>
    <dd><prep>On branch main<br/>
    Your branch is ahead of 'origin/main' by 2 commits.<br/>
      (use "git push" to publish your local commits)<br/><br/>
    nothing to commit, working tree clean</prep></dd>
     
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>
$ git log --oneline</dt>
<dd></dd>9fc4abc (HEAD -> main) Merge branch 'main' of https://github.com/Lu1sMig/sistema-de-registro
6bc3db7 (origin/desarrollo, desarrollo) agregando instructor datos
03e62db (origin/main, origin/HEAD) Update app.js
29e13a1 Actualiza nombre app.js y en link en index.html
83a55b0 archivo contacto
0569fe7 Update README.md
470b8bf crea el index .html
9f18c9c actualiza README.md
32b8a07 Update README.md
85a557a Crea el app-js
b6adac0 Update README.md
502493f Create README.md</dd>

SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)
$ git merge desarrollo
Already up to date.

SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)
$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 313 bytes | 313.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Lu1sMig/sistema-de-registro.git
   03e62db..9fc4abc  main -> main
</dd>
<li>Profundizando en Git y GitHub</li>
<dl>
  <dd>
    <prep>Aprendimos que hay otra forma de iniciar un repositorio Git, además de clonar uno existente. Se puede hacer usando el comando "git init" en una carpeta vacía.

Después de inicializar el repositorio local con "git init", creamos un archivo HTML básico y lo agregamos al repositorio con "git add" y "git commit".

Para conectar el repositorio local con un repositorio remoto en GitHub, usamos el comando "git remote add" para establecer la URL del repositorio remoto.

Actualizamos la rama principal de "master" a "main" usando el comando "git branch -M main".

Finalmente, enviamos los cambios al repositorio remoto usando "git push -u origin main". La opción "-u" nos permite usar después sólo "git push" para enviar futuros cambios.
Los comandos utilizados en esta clase fueron:

git init - Inicializa un nuevo repositorio Git en la carpeta actual.

git add - Agrega archivos al área de preparación (staging area) para ser incluidos en el próximo commit.

git commit - Crea un nuevo commit con los cambios preparados.

git remote add - Conecta el repositorio local con un repositorio remoto en GitHub.

git branch -M main - Cambia el nombre de la rama principal de "master" a "main".

git push -u origin main - Envía los commits del repositorio local al repositorio remoto en GitHub. La opción "-u" establece "origin main" como rama predeterminada para futuros pushes.

git remote -v - Muestra las URLs de los repositorios remotos configurados.
  </prep></dd>

  <dt>
    Subiendo repositorio desde equipo
  </dt>
  <dd>
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro2 (master)<br/>
$ git init</dt>
<dd>Initialized empty Git repository in C:/Users/SOPORTE/Documents/GitHub/sistema-de-registro2/.git/</dd>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro2 (master)<br/>
$ code .</dt>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro2 (master)<br/>
$ git add .</dt>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro2 (master)<br/>
$ git status</dt>
<prep>On branch master
No commits yet
Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html</prep>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro2 (master)<br/>
$ git commit -m "crea index"</dt>
<prep>[master (root-commit) b4bf636] crea index
 1 file changed, 11 insertions(+)
 create mode 100644 index.html
</prep>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro2 (master)<br/>
$ git remote add origin https://github.com/Lu1sMig/sistema-de-registro2.git</dt>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro2 (master)<br/>
$ git branch -M main</dt>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro2 (main)<br/>
$ git push -u origin main</dt>
<prep>Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 373 bytes | 373.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Lu1sMig/sistema-de-registro2.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.</prep>

  </dd>
</dl>
</li>
<li>Resumen de Modulo
  <dl>
    En la clase se presentaron los siguientes comandos de Git:
Para configurar:
git config global user.name y user.email: para configurar el nombre y correo electrónico del usuario.
git config --list: para ver las configuraciones actuales de Git.
    
Para crear repositorio:    
git clone: para clonar un repositorio remoto.
git init: para inicializar un nuevo repositorio local.

Para Verificar 
git status: para ver el estado actual del repositorio.
git log: para ver el historial de commits.
git diff: para ver los cambios en los archivos.
git branch: para ver las ramas existentes.

Para Agregar:
git add .       : para agregar todos los archivos al área de preparación (staging area).
git add [file]  : para agregar un archivo especifico al área de preparación (staging area).

Para Mover:
git commit: para crear un nuevo commit con los cambios.
git push: para enviar los commits al repositorio remoto.
git pull: para traer los cambios del repositorio remoto.

Para cambiar:
git checkout -b: para crear una nueva rama.
git merge: para fusionar una rama con otra.
git switch: para cambiar de una rama a otra.
git restore --source [hash] [archivo]: para volver a un estado de commit anterior.
  </dl>
</li>
</ol>


<style type=”text/css”>
ol {  list-style-type: lower-roman;}
</style>

