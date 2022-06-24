# Resumo de comando GIT e GITHUB
![Alt text](command-git.jpg?raw=true "Resumo de comando GIT e GITHUB")

Git é sistema de controle de Versão Distribuído

# 1. Local de operações do Git:
## 1.1 - Working Directory
## 1.2 - Staging Area
## 1.3 - Git Directory (repositório)

## flow: Working Directory [git add] >> Staging Area [git commit] >> Git Directory
## 1.4 - Quick setup — create a new repository or existing repository
   ### 1.4.1 -> create a new repository on the command line
	echo "# rest-api-with-docker-mongdb" >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git branch -M master
	git remote add origin git@github.com:gleideveloper/rest-api-with-docker-mongdb.git
	git push -u origin master

   ### 1.4.2 -> push an existing repository from the command line
	git remote add origin git@github.com:gleideveloper/rest-api-with-docker-mongdb.git
	git branch -M master
	git push -u origin master

# 2. Configuração Inicial do Git - Sua Identidade

	$ git config --global user.name "Gleides Vinente"
	$ git config --global user.email "gleidesigner@msn.com"

## 2.1 Verificando Suas Configurações

	$ git config --list

# 3. Obtendo Ajuda - Existem três formas:

	$ git help <verb>
	$ git <verb> --help
	$ man git-<verb>

## 3.1 Exemplo:

	$ git help config

# 4. Git Essencial - Obtendo um Repositório Git

	$ git init
	$ git clone git@github.com:user-name-git/nome-repositorio-remoto.git

## 4.1 Exemplo:

	$ git clone git@github.com:gleidesigner/curso_git.git


#Comandos básicos do Git

Adicionar um arquivo na Staging Area

	$ git add.

Remover um arquivo da area Staging
	
	$ git rm --cached

Remover um arquivo do repositório local
	
	$ git rm NomeDoArquivo


Adicionar um arquivo na area Git Directory

	$ git commit -m "informação sobre o commit"

Mostrar a diferença no arquivo
	
	$ git diff

Mostrar a diferença no arquivo na Staging Area

	$ git diff --staged

Mostrar o log de todos os commits do projeto

	$ git log

Mostrar o log de todos os commits com detalhes da mudança do projeto

	$ git log -p

Mostrar o log de n(numero de logs) commits do projeto

	$ git log -p -1

Informar apenas o log e informações dos commits do projeto

	$ git log --pretty=oneline 

Adiciona as mudanças no último commit feito no projeto
	
	$ git commit --amend -m "informações"

Descartas as ultimas mudanças feitas no arquivo

	$ git checkout -- NomeDoArquivo

Criar branch no repositório local

	$ git branch NomeDoBranch

Alterar o branch no repositório local

	$ git checkout NomeDoBranch

Criar e alterar um branch no repositório local

	$ git checkout -b NomeDoBranch

Fazer um merge entre os branchs (teste2 para o master), deve-se está no branch master e vice-versa

	$ git merge teste2

Deletar o branch no repositório local

	$ git branch -d NomeDoBranch

Enviar mudanças do repositório local para o remoto

	$ git push origin master

Pegar as mudanças do repositório remoto

	$ git pull origin master


webgrafia: fonte: https://git-scm.com/book/pt-br/v1
