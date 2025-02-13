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
$ git config --list<br/>
diff.astextplain.textconv=astextplain<br />
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
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br />$ git status</dt>
<dd>On branch main<br/> Your branch is up to date with 'origin/main'.<br/>Untracked files:<br/>  (use "git add <file>..." to include in what will be committed)<br/>contacto.html<br/>
nothing added to commit but untracked files present (use "git add" to track)
</dd>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>$ git add .</dt>
<dd></dd>
<dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>$ git commint -m "archivo contacto"</dt>
<dd>git: 'commint' is not a git command. See 'git --help'.<br/><br/><br/>The most similar command is<br\>commit </dt></dd>
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
  </li>
  <dl>
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>$ git branch<br/></dt>
    <dd>* main</dd><
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br>$ git checkout -b desarrollo</dt>
    <dd>Switched to a new branch 'desarrollo'</dd>
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)<br>$ git switch main</dt>
    <dd>Switched to branch 'main'<br/>Your branch is up to date with 'origin/main'.</dd>
    <dt>SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (main)<br/>$ git branch</dt>
    <dd>desarrollo<br/>* main</dd>
  </dl>

SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)
$ git add .

SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)
$ git commit -m "agregando instructor datos"
[desarrollo 6bc3db7] agregando instructor datos
 1 file changed, 1 insertion(+)

SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)
$ git push
fatal: The current branch desarrollo has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin desarrollo

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)
$ git push origin desarroll
error: src refspec desarroll does not match any
error: failed to push some refs to 'https://github.com/Lu1sMig/sistema-de-registro.git'

SOPORTE@MPFNMPF-GAKM4HB MINGW64 ~/Documents/GitHub/sistema-de-registro (desarrollo)
$ git push origin desarrollo
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
 * [new branch]      desarrollo -> desarrollo

      
</ol>


<style type=”text/css”>
ol {  list-style-type: lower-roman;}
</style>

