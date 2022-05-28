## CURSO GIT

### GitHub Commands:
<img alt="github_logo" src="https://github.githubassets.com/images/modules/logos_page/Octocat.png" width="100" height="100">

- Creates a online repository:

  ``gh repo create``<br/>
  - E.g: 
    - 1º: Create a new repository on Github from scratch
    - 2º: Push an existing local repository to GitHub
      - Path to local repository (default is "." current path)
      - Repository name (default is FolderName)
      - Visibility:
        - Public: Accessible to everyone in internet
        - Private: Only accessible to you, people you explicitly share access with and or Organization repositories, certain organization members
        - Internal: Internal repositories are accessible to all enterprise members
      - Add a remote: (yes=Add a new remote connection config to current git project, no=Don't add remote connection config)
      - What should the new remote be called (default is origin)
      - Would you like to push commits from the current branch to "origin"? (y=Push commits to previously configured remote, n=Don't push commits)
      
### GIT Commands:

<img alt="git_logo" src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png" width="100" height="100">

- Creates a local repository in current cli context folder:

  ``git init``


- Repository status in current moment:

  ``git status``<br/>
  ``git status -uall``<br/>
  E.g: -uall Show the hierarchy of dirs and subdirs to be added, updated or removed.


- Repository changes using LOG gives a more detailed information with file contents:

  ``git log``

- Add new files/dirs in repository:

  ``git add file.txt``


- Remove files/dirs from repository (Unstage):

  ``git rm --cached file.txt|folder``

  E.g: --cached Remove from repository
       without --cached delete from repository and from pc


- Salvar alterações (Commit):

  ``git commit -m "Primeiro commit"``

  ``git commit -a -m "Commit alterações"``


- Pull changes from remote:

  ``git pull``

- Push changes to remote:

  ``git push origin main``


- Configure GIT email and user name:

  ``git config --global user.name "Meu Nome de Usuário"``

  ``git config --global user.email "seu@email.com"``


- Configure default GIT branch:

  ``git config --global init.defaultBranch main``


- List configurations from git project:

  ``git config --list``


- Show changes in current BRANCH (Changes from respository):

  ``git show``


- Show changes in a specific file. (Changes from remote and local changes):

  ``git diff index.html``


- Git Ignore (Ignora pastas e arquivos que não vão ser versionados):

  ``.gitignore``

  
- Change current branch:

  ``git branch -M main``
  

- List git remote repos name | url:

  ``git remote -v``


- Add new git remote po name | url:

  ``git remote --add origin https://github.com/user-name/repo-name.git``


- Save old commits in a new branch before Overwriting:

  ``git checkout master``

  ``git branch ``


- Overwrite local changes using repo changes:

  ``git fetch --all``

  ``git reset --hard <remote>/<branch>``
