## CURSO GIT

### Comandos:
- Criar um repositório local:

  ``git init``


- Status do repositório no momento:

  ``git status``


- Adicionar arquivos/pastas no repositório:

  ``git add file.txt``


- Remover arquivos/pastas do repositório (Unstage):

  ``git rm --cached file.txt|folder``

  OBS: --cached Remove do repositório
       sem o cached remove do repositório e do pc


- Salvar alterações (Commit):

  ``git commit -m "Primeiro commit"``

  ``git commit -a -m "Commit alterações"``



- Configurações GIT nome do usuário e o email:

  ``git config --global user.name "Meu Nome de Usuário"``

  ``git config --global user.email "seu@email.com"``


- Listar configurações atuais:

  ``git config --list``


- Exibir as alterações de arquivos do BRANCH atual (Alterações do repositório):

  ``git show``


- Exibir as alterações em um arquivo específico. (Diferenças do repositório com as alterações locais):

  ``git diff index.html``


- Git Ignore (Ignora pastas e arquivos que não vão ser versionados):


  ``.gitignore``