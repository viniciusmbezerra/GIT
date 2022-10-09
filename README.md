# GIT

[Lista de comandos avançados](https://gist.github.com/leocomelli/2545add34e4fec21ec16)

## ``Comandos fundamentais do git``

Criar repositório
```
git init
```

Adicionando origem
```
git remote add origin https://github.com/
git branch -M main
git push -u origin main
```
Conexão com ssh
```php
ssh-keygen //no terminal local
//Your public key has been saved in C:\Users\vinic/.ssh/id_rsa.pub.
cat C:\Users\usuario/.ssh/id_rsa.pub //pegando chave pública
//adicionar chave no github e no remote local
git remote add origin git@github.com:teste/teste.git
```

Clonar
```
git clone https://github.com/
```

Verificar mudanças, apresentando informações da branch
```
git status
git show
git show nome_branch
```
Exibindo diferenças
```
git diff nome_branch
git diff nome_branch:arquivo1 nome_branch:arquivo2
```

Adicionar arquivos
```
git add .
git add nome_aquivo
```

Salvando alterações
```
git commit -a -m 'msg'
git commit nome_arquivo -m 'msg'
```

Enviando e buscando | GitHub
```
git push
git pull
```

Deletar arquivo | diretório
```
git rm nome_arquivo
git rm -r nome_dir
```

Histórico de alterações
```
git log
git shortlog
```

Renomeando arquivos e diretórios
```
git mv nome_atual nome_novo
```

Desfazendo alterações de um arquivo antes do commit
```
git checkout nome_arquivo
```

Ignorando arquivos e diretórios
```
coloque no .gitignore
```

Desfazendo todas as alterações de uma branch
```
git reset --hard nome_branch
```

## ``Branch``

Criar, deletar, mudar branchs
```
git branch nome_branch
git branch -D nome_branch
git checkout nome_branch
```
Criar e mudar para uma branch
```
git checkout -b nome_branch
```
Listar branchs remotas
```
git branch -r
```
Listar branchs remotas e locais
```
git branch -a
```
Listar branchs com detalhes
```
git branch -v
```

Renomear branch
```
git branch -m nome_atual nome_novo
```

``Sempre faça o commit antes de mudar de branch``

Unir branchs
```
git merge nome_branch
```
Buscando, enviando, deletando | GitHub
```
git fetch
git pull

git push --set-upstream nome_branch

git push --delete origin nome_branch
```

## ``Stash``

Salva modificações atuais de uma branch sem perder o código

Criando, Listando, Recuperando, Apagando todas, Apagando uma
```
git stash
git stash list
git stash nome_stash
git stash clear
git stash drop nome_stash
```

## ``Tags``

Cria checkpoints na branch atual

Criando
```
git tag -a nome_tag -m 'mensagem'
git tag nome_tag
```

Mostrando, Mudando e Deletando
```
git show nome_tag
git checkout nome_tag
git tag -d nome_tag
```

Buscando, enviando, deletando | GitHub
```
git fetch
git pull

git push origin nome_tag
git push origin --tags

git push --delete origin nome_tag
```

## ``Submódulos``
Repositórios dentro de repositórios

Listar, Adicionar, Enviando para o remoto, Atualizando
```
git submodule
git submodule add https://github.com/
git push --recurse-submodules=on-demand
git pull
```
