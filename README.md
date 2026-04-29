# Aula de Git

## Criação de primeiro repositório



### Inicia o git

$ git init
Initialized empty Git repository in C:/Users/Dell/Documents/GitHub/Aula0301/.git/

### Nome do usuário

$ git config --global user.name "orlandovcj"

### E-mail do usuário

$ git config --global user.email "orlandovcj@gmail.com"

### Mostra o status do repositório

$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

### Muda o nome do main branch

$ git config --global init.defaultBranch main

### Adiciona um arquivo no repositório

$ git add README.md

### Cria um commit do arquivo para o repositório

$ git commit -m "Primeiro commit: criação do README"
[main (root-commit) 82e9a4f] Primeiro commit: criação do README
 1 file changed, 2 insertions(+)
 create mode 100644 README.md

### Mostra o log de alterações

$ git log
commit 82e9a4f4027c40f65faf2cc89b2d76796c936205 (HEAD -> main)
Author: orlandovcj <orlandovcj@gmail.com>
Date:   Tue Apr 28 21:22:39 2026 -0300

    Primeiro commit: criação do README

### Mostra o status atual depois de atualização do arquivo

$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

### Adiciona uma nova atualização

$ git add README.md

### Faz o commit da autualização

$ git commit -m "Atualização de conteúdo"
[main 17e8d5d] Atualização de conteúdo
 1 file changed, 53 insertions(+), 1 deletion(-)

### Mostra o log de atualização

$ git log
commit 17e8d5decd26f246721ae21b2f0c07bd6cfdef92 (HEAD -> main)
Author: orlandovcj <orlandovcj@gmail.com>
Date:   Tue Apr 28 21:34:12 2026 -0300

    Atualização de conteúdo

commit 82e9a4f4027c40f65faf2cc89b2d76796c936205
Author: orlandovcj <orlandovcj@gmail.com>
Date:   Tue Apr 28 21:22:39 2026 -0300

    Primeiro commit: criação do README

### Log com o parâmetros --oneline exibe os commits

$ git log --oneline
17e8d5d (HEAD -> main) Atualização de conteúdo
82e9a4f Primeiro commit: criação do README
