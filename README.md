# Teste

Comandos-Git-bash
Comandos básicos para se utilizar no Git, e um pequeno guia de como utilizá-los!
Índice
Nome e Usuário
Clonando um Repositorio Existente
Gravando Alterações
Commits
Histórico de Commits
Limpar a Tela

1 - Nome e Usuário
A primeira coisa que você deve fazer quando instalar o Git é definir o seu nome de usuário e endereço de e-mail. Isso é importante porque todos os commits no Git utilizam essas informações, e está imutavelmente anexado nos commits que você realiza:

git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
=======================================================================================


2 - Clonando um Repositorio Existente
Você clona um repositório com git clone [url]. Utilizamos esse comando na ultima aula prática do curso

"Criando seu Primeiro Repositorio no Github Para Compartilhar Seu Progresso"
git clone [url]
=======================================================================================


3 - Gravando Alterações
Quando um repositório é inicialmente clonado, todos os seus arquivos estarão monitorados e inalterados porque você simplesmente os obteve e ainda não os editou. Conforme você edita esses arquivos, o Git passa a vê-los como modificados, porque você os alterou desde seu último commit. Você seleciona esses arquivos modificados e então faz o commit de todas as alterações selecionadas e o ciclo se repete.

Para passar a monitorar um novo arquivo, use o comando git add. Para monitorar o arquivo README, você pode rodar isso:

git add README
=======================================================================================


4 - Commits
Armazena o conteúdo atual do índice em um novo commit, juntamente com uma mensagem de registro do usuário que descreve as mudanças. Se usa o commit depois de já ter feito o git add, para fazer o commit:

git commit -m "Mensagem"
Para commitar também os arquivos versionados mesmo não estando no Stage basta adicionar o parâmetro -a
git commit -a -m "Mensagem"
Refazendo commit quando esquecer de adicionar um arquivo no Stage:
git commit -m "Mensagem" --amend
O amend é destrutivo e só deve ser utilizado antes do commit ter sido enviado ao servidor remoto.
=======================================================================================


5 - Histórico de Commits
Depois que você tiver criado vários commits, ou se clonou um repositório com um histórico de commits existente, você provavelmente vai querer ver o que aconteceu. A ferramente mais básica e poderosa para fazer isso é o comando:

git log
=======================================================================================


6 - Limpar a Tela
Para limpar a tela do Git, basta pressionar

CTRL + L
.
=======================================================================================

Link úteis:
Lista de comandos básicos
