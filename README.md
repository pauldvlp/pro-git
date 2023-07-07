```
# Commands
> git config --global user.name 'My name'
> git config --global user.email 'my-email@website.com'
> git config --global alias.unstage 'reset HEAD'
> git config --global alias.oneline 'log --pretty=oneline'
> git config --global alias.st status
> git config --global alias.s 'status -sb'
> git config --global alias.undo 'checkout --'
> git config --global alias.last 'log -1 HEAD --stat'
> git config --global alias.dt 'difftool'
> git config --global alias.alias '!f() { git config --global alias.$1 "$2"; }; f'
> git init
> git clone [url] ?[dirname]
> git status (--short/-s)
> git add [path]
> git mv [file-from] [file-to]
> git diff (--staged)
> git commit (-a) (-m) (--amend)
> git rm (-f) (--cached) [path]
> git log (-p) (-2) (--stat) (--pretty=oneline|short|full|fuller|format) (--graph) (--decorate)
> git reset HEAD [file]
> git checkout -- [file]
> git remote (-v) (show) (add) (rename) (rm)
> git fetch
> git push (--tags)
> git pull
> git tag (-l) (-a) (-m)
```

```
.gitignore

# ignora los archivos terminados en .a
*.a

# pero no lib.a, aun cuando había ignorado los archivos terminados en .a en la línea
anterior
!lib.a

# ignora unicamente el archivo TODO de la raiz, no subdir/TODO
/TODO

# ignora todos los archivos del directorio build/
build/

# ignora doc/notes.txt, pero no este: doc/server/arch.txt
doc/*.txt

# ignora todos los archivos .txt del directorio doc/
doc/**/*.txt
```

```
git log format options

| Opción | Descripción de la salida |
| %H     | Hash de la confirmación
| %h     | Hash de la confirmación abreviado |
| %T     | Hash del árbol |
| %t     | Hash del árbol abreviado |
| %P     | Hashes de las confirmaciones padre |
| %p     | Hashes de las confirmaciones padre abreviados |
| %an    | Nombre del autor |
| %ae    | Dirección de correo del autor |
| %ad    | Fecha de autoría (el formato respeta la opción -–date) |
| %ar    | Fecha de autoría, relativa |
| %cn    | Nombre del confirmador |
| %ce    | Dirección de correo del confirmador |
| %cd    | Fecha de confirmación |
| %cr    | Fecha de confirmación, relativa |
| %s     | Asunto |
```

```
# Use VS Code as Difftool

git config --global diff.tool vscode
git config --global difftool.vscode.cmd 'code --wait --diff $LOCAL $REMOTE'
```