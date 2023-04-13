## GIT COURSE

### GitHub Commands:
<img alt="github_logo" src="https://github.githubassets.com/images/modules/logos_page/Octocat.png" width="100" height="100">

- Create a online repository:

  ``gh repo create``<br/>
  - **E.g:**
    - 1º: Create a new repository on Github from scratch
    - 2º: Push an existing local repository to GitHub
      - Path to local repository (default is "." current path)
      - Repository name (default is FolderName)
      - **Visibility:**
        - **Public:** Accessible to everyone in internet
        - **Private:** Only accessible to you, people you explicitly share access with and or Organization repositories, certain organization members
        - **Internal:** Internal repositories are accessible to all enterprise members
      - **Add a remote:** (**y**=Add a new remote connection config to current git project, **n**=Don't add remote connection config)
      - What should the new remote be called (default is origin)
      - Would you like to push commits from the current branch to "origin"? (**y**=Push commits to previously configured remote, **n**=Don't push commits)

### GIT Commands:

<img alt="git_logo" src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png" width="100" height="100">

- Creates a local repository in current cli context folder:

  ``git init``


- Repository status in current moment:

  ``git status``

  ``git status -uall``

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

- List branches:

  ``git branch``

- Create a new branch as a copy of current branch:

  ``git switch -c new-branch``


- Change current branch:

  ``git branch -M main``


- Delete branch:

  ``git branch -d branch-name``


- Delete remote branch:

  ``git branch -rd branch-name``

- List local and remote branches:

  ``git branch -a``


- Push a new branch to it's upstream:
  
  ``git push --set-upstream origin branch_name``


- List git remote repos name | url:

  ``git remote -v``


- Add new git remote po name | url:

  ``git remote add origin https://github.com/user-name/repo-name.git``


- Switch branch to (Rollback / Forward) changes to a specific commit(using commit hash) in git log:

  ``git checkout b451asd``


- Switch to a new branch and create it:

  ``git checkout -b main``


- Switch to a existing branch:

  ``git checkout -b main``


- Save old commits in a new branch before Overwriting:

  ``git checkout main``

  ``git branch my-brach-name``


- Overwrite local changes using repo changes:

  ``git fetch --all``

  ``git reset --hard <remote>/<branch>``


- If some error happens create a temporary branch commit changes in it
  then get changes from main and merge this two branches

  ``git branch temp-branch``

  ``git checkout main``

  ``git merge temp-branch``

  ``git push origin master``


- Solving Merge Conflicts
- After pulling the changes when a conflict occurs the conflict is shown in the files
in this format:

  ```
  print("Ola mundo")
  <<<<<<< HEAD
  print("My new line")
  =======
  print("Nova linha")
  >>>>>>> 8050fd126537c51cd5288e5b40dfcd2aa66528e4
  ```
  ```
  - From line <<<<< HEAD until line ====== Are your version changes in the file.
  - From line ===== until >>>>>>> 8050fd126537c51cd5288e5b40dfcd2aa66528e4 are the other
  commit that is conflicting at same lines in your commit files.
  ```
  - Fix the issue in the file by deleting the changes you don't want
and keeping the changes you want then run the commands:
  
  ``git commit -m "Commit description"``

  ``git push``
