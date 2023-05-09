# Controle de versão
Forma de controlar a vesão do codigo de forma automatizada

VCS - Version Control System
 - gerenciar o historico da alteraçoes que os arquivos do nosso projeto
 sofreu ao longo do tempo

 # GIT
  O git foi inicilamente um projeto desenvolvido para o desenvovimento
  do Kernel Linux, mas foi adotado por muitos outros projetos e atualmente
  é o melhor controlador de versões mais utilizados.

  # comandos git
  - git init: inicializar um projeto git, que o git vai versionalizar o projeto.
  
  - The .git: um arquivo invisivel(escondido) na nossa aplicação onde fica todos os
  arquivos de configuração que o git usa para armazenar todo o historico de alteraçoes ao longo
  do desenvolvimento da aplicção(!inportant não apagar por isso que ela fica oculta)

  # configurando o git 
  - 1* o nome: git config --global user.name "davi"
  - 2* email: git config --global user.email "davihenrique@example.com.br"

  - git config --list: ele vai listar qual o conteudo do arquivo de configuraçoes do git.
  - apertando a tecla q ele vai sair

  # primeiro commit 
  -- O que é:
  -um ponto na historia que vc sinaliza que aconteceu alguma coisa importante 
  - git add . : ele vai adicionar todos os arquivos que sofreram algum tipo de atualizaçao
  - git commit -m "create project": é como se fosse uma identificação falando que tem alí(o que ele faz)
  sempre escrever mesnsagem curta e objetivas
  
  # Git log
  ver os historicos de commit já feito 
  -git log: traz todos os commits ja feito
  ele tras um indentificador(todo commit tem)
  o autor(que editou)
  e quando (Hora e dia)
  e a mensagem
  press q for the end(sair)

  - git log --oneline: é a forma mais resumida de ver o log

  -- uma coisa legal tambem é uma forma de trazer uma forma definida de log,
  as vezes fazemos varios commits e vc não quer que traga todos, somente os 3 ultimos logs:
  -git log -n 3 (quantos commits quer que mostre)

 # git diff
 Vai ajudar a comparar as mudanças q foi feita com o atual e o ultimo commit
  -git diff: vai mostrar o que mudou(qual o conteudo exato que foi modificado antes/depois)

  # desfazendo auteraçoes
  quando vc quer desfazer alguma alteração que deu errado e/ou não só em um unico arquivo
  -git restore 'nome do arquivo': restaurar um unico arquivo
  git restore . : restaurar todos os arquivos

  # Repositorios remotos
   *git pull
   repositorios remotos que qundo uma pessoa que vc compartilhou o código e a modificou vc trás para a sua maquina aquele arquivo alterado

# Git branche
 - git branch master: comando para criar um branch com o nome master
 - git checkout teste: comando pra mudar a banch de master para teste

 - git log --oneline --decorate: comando para mostrar em em que branch estamos
 -git merge: comando para juntar todas as branch disponiveis na master