# Git e Github
> Tutorial de como configurar e usar Git e Github

## Configurações iniciais

Primeiro passo, vamos configurar seu nome e email no Git.

1. Adicionando nome:
```git
git config --global user.name "Fulano de Tal"
```
2. Para confirmar a mudança do nome:
```git
git config user.name
```
3. Adicionando email:
```git
git config --global user.email fulanodetal@exemplo.br
```
4. Para confirmar a mudança do email:
```git
git config user.email
```

## Iniciando o Git em um diretório e linkando com o Github

Segundo passo, entre no diretório desejado e use os comandos abaixo:

1. Criando o README.md:
```git
echo "# NOME_DO_ PROJETO" >> README.md
```
2. Iniciando o git:
```git
git init
```
3. Adicionando o README.md ao stage:
```git
git add README.md
```
4. Commitando as mudanças:
```git
git commit -m "first commit"
```
5. Defindo a branch Main como principal:
```git
git branch -M main
```
6. Linkando o diretório local com o diretório no Github:
```git
git remote add origin https://github.com/USER_NAME/REPOSITORY_NAME.git
```
7. Sincronizando ambos diretóriosna branch Main:
```git
git push -u origin main
```

## Git comandos principais

Mostrar se tem arquivos modificados que precisam ir para o stage:
```git
git status
```

Mostrar as modificações feitas:
```git
git diff 
git diff NOME_ARQUIVO
```

Adicionar no stage:
```git
git add NOME_ARQUIVO
```

Removendo arquivos do Stage:
```git 
git reset
```

Criar commit:
```git
git commit -m "MENSAGEM"
```

Adicionar no stage e criar commit:
```git
git commit -a -m "MENSAGEM"
```

Desfazendo o último commit:
```git
git revert HEAD
```

Renomear Commit:
```git
git commit --amend
```

Desfazer alterações até voltar ao ultimo commit de arquivos:
```git
git checkout .
git checkout NOME_ARQUIVO
```

Limpar diretórios fora do stage:
```git
git clean -f
```

Criar nova branch:
```git
git checkout -b "NOME_BRANCH"
```

Excluindo branches:
```git
git branch -d NOME_BRANCH
```

Renomeando branches:
```git
git branch -m NOVO_NOME_BRANCH
```

Renomeando branches vizinhas:
```git
git branch -m NOME_ATUAL_BRANCH NOVO_NOME_BRANCH
```

Criar branch no repositório remoto e enviar as mudanças para lá:
```git
git push --set-upstream origin NOME_BRANCH
```

Enviar os novos commits para a branch já existente:
```git
git push
```

Trocar de branch:
```git
git checkout NOME_BRANCH
```

Listar todas as branchs:
```git
git branch
```

Ver histórico de commits:
```git
git log
```

Unir códigos de duas branchs localmente:
```git
git merge NOME_BRANCH
```

Depois de unir basta usar o comando:
```git
git push
```

> *Agora você enviou o merge para o github.*

Atualizar repositório local:
```git
git pull
```

Histórico de um ou mais arquivos:
```git
git log -p MEUS_ARQUIVOS
```

Histórico de um autor:
```git
git log --autor=NOME_AUTOR
```




