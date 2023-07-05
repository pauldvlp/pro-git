```
# Commands
> git config --global user.name 'My name'
> git config --global user.email 'my-email@website.com' 
> git init
> git clone [url] [dirname]
> git status (--short/-s)
> git add [path]
> git diff (--staged)
> git commit (-a) (-m)
> git rm (-f) (--cached) [path]
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