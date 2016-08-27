#Curso Git linhas de comando

Git é sistema de controle de Versão Distribuído

# 1. Local de operações do Git:
## 1.1 - Working Directory
## 1.2 - Staging Area
## 1.3 - Git Directory (repositório)

## flow: Working Directory [git add] >> Staging Area [git commit] >> git directory

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

#3.2 Exemplo:

$ git clone git@github.com:gleidesigner/curso_git.git



#webgrafia: fonte: https://git-scm.com/book/pt-br/v1