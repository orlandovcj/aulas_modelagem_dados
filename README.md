# Aula de Git

## Criação de primeiro repositório



Dell@DESKTOP-DPMILID MINGW64 ~/Documents/GitHub/Aula0301
$ git init
Initialized empty Git repository in C:/Users/Dell/Documents/GitHub/Aula0301/.git/

Dell@DESKTOP-DPMILID MINGW64 ~/Documents/GitHub/Aula0301 (master)
$ git config --global user.name "orlandovcj"

Dell@DESKTOP-DPMILID MINGW64 ~/Documents/GitHub/Aula0301 (master)
$ git config global user.email "orlandovcj@gmail.com"
error: key does not contain a section: global

Dell@DESKTOP-DPMILID MINGW64 ~/Documents/GitHub/Aula0301 (master)
$ git config --global user.email "orlandovcj@gmail.com"

Dell@DESKTOP-DPMILID MINGW64 ~/Documents/GitHub/Aula0301 (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

Dell@DESKTOP-DPMILID MINGW64 ~/Documents/GitHub/Aula0301 (master)
$ git branch -m master main

Dell@DESKTOP-DPMILID MINGW64 ~/Documents/GitHub/Aula0301 (main)
$ git config --global init.defaultBranch main

Dell@DESKTOP-DPMILID MINGW64 ~/Documents/GitHub/Aula0301 (main)
$ git add README.md

Dell@DESKTOP-DPMILID MINGW64 ~/Documents/GitHub/Aula0301 (main)
$ git commit -m "Primeiro commit: criação do README"
[main (root-commit) 82e9a4f] Primeiro commit: criação do README
 1 file changed, 2 insertions(+)
 create mode 100644 README.md

Dell@DESKTOP-DPMILID MINGW64 ~/Documents/GitHub/Aula0301 (main)
$ git log
commit 82e9a4f4027c40f65faf2cc89b2d76796c936205 (HEAD -> main)
Author: orlandovcj <orlandovcj@gmail.com>
Date:   Tue Apr 28 21:22:39 2026 -0300

    Primeiro commit: criação do README
