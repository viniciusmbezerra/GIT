# GIT

## ``Comandos fundamentais do git``

Criar repositório
```
git init
```

Adicionando origem
```
git remote add origin https://github.com/viniciusmbezerra/GIT.git
git branch -M main
git push -u origin main
```

Clonar
```
git clone https://github.com/viniciusmbezerra/GIT.git
```

Verificar mudanças
```
git status
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

Deletar arquivo
```
git rm nome_arquivo
```

Histórico de alterações
```
git log
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

Desfazendo todas as auterações de uma branch
```
git reset --hard nome_branch
```

## ``Branch``

Criar, listar, deletar, mudar branchs
```
git branch nome_branch
git branch
git branch -D nome_branch
git checkout nome_branch
```
Criar e mudar para uma branch
```
git checkout -b nome_branch
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

