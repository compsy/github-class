name: inverse
layout: true
class: center, middle, inverse

---
# GitHub Workshop

### Ando Emerencia and Frank Blaauw
#### University of Groningen,<br/>Developmental Psychology / Computer Science

---
layout: false

# Outline

- Why do I need git?
- Introduction to git and GitHub
- How do we use git?
- Hands-on workshop

---

# Why do I need git?

- Code History
- Reverting changes
- Collaborating with colleagues
- Code review

---

# For what is git useful?

- Version Control System
- Managing plain text files (R syntax, Matlab files, source code, txt files)

# For what is git not useful?

- Managing microsoft office documents
- Storing data

???
Git is a version management system, which means that it can keep track of earlier versions of your source code / documents.

---

# The git basics

- Clone
- Pull
- Add
- Commit
- Push

---

# Repositories

.center[
  ![Git flow](images/git-flow.png)
]

- (cloud hosted) remote location containing your code.
- GitHub is a provider of hosted git repositories.

---

# Clone

.center[
  ![Git flow](images/git-flow.png)
]

- Downloading a remote repository to your local machine.
- Only do this once the first time.
---

# Pull

.center[
  ![Git flow](images/git-flow.png)
]

- Updating your local clone with the latest version from the git provider.
- Do this every time you want to _pull in_ changes from the remote repository.

---

# Add / stage

.center[
  ![Git flow](images/git-flow.png)
]

- Selecting files / changes that you would like to store in git.
- You will have to do this every time you want to store changes or files.

---

# Commit

.center[
  ![Git flow](images/git-flow.png)
]

- With a commit you can combine all the staged files into a single update.
- A commit comes with a commit message. In these messages you can write what you changed and why you changed something.

---

# Push

.center[
  ![Git flow](images/git-flow.png)
]

- With a push you upload your commits to the git provider (in our case GitHub)
- You have to push in order to share your commits with everyone.

---

# Branching - the master

.center[
  ![Master](images/master.png)
]

Supposed to be the _stable_ version of the code.

---

# Branching - a feature branch

.center[
  ![Branch](images/branch.png)
]

---

# Branching - Pull request

.center.small[
  ![Branch](images/pull-request.png)
]

Moment to _review code_ before merging it to master.

---

# Branching - merged

.center[
  ![Branch](images/merged.png)
]

A pull request causes the change to be merged into master.

---

# A basic collaboration workflow

- Clone a repository.
- Create a new branch.
- Make changes in that branch and add / commit / push to GitHub.
- Create a pull request and ask others to review the changes.
- If changes are ok, merge the branch into master.

---

# Other, more advanced topics (not discussed today)

- Git has a powerful command line interface
- You can use public / private key SSH keys instead of using a username and password
- GitHub can be combined with various services for automatically performing running tests on the code in GitHub (e.g., CircleCI)

---

name: inverse
layout: true
class: center, middle, inverse
---
# Hands on
---

layout: false

# Signing in to MyUWP

- Open https://uwp.rug.nl and login
- Click on _Workspace desktop_
- When you are logged in, start the Google Chrome browser
- All the next steps should be performed from within the UWP client.

---

# Creating a GitHub repository

- Log in on https://github.com
- Click on the green _New_ button next to _Repositories_
  - Fill in a name for the repository
  - Description is not necessary
  - Make it a public repository
  - No need to initialize it with anything
  - Click on _Create repository_
- Click on the clipboard button to copy the repository url.

---

# Install git

- Go to https://git-scm.com/download/win and download the installer.
- Keep clicking next until it starts installing.

---

# Configuring R Studio to work with git
- Open the Windows start menu, type: `R studio`
- In R Studio, Open the Tools menu and select Global options
  - Go to Git/SVN
  - Browse to the correct git executable (e.g. _C:/Users/pnumber/AppData/Local/Programs/Git/bin/git.exe_)
  - Click OK
- Close R Studio

---

# Cloning a repository in R Studio

- Open R Studio again
- Go to _File_ and select _New project_
  - Select _Version control_
  - Click on  _Git_
  - Paste the repository URL
  - (optional) change the directory to store the code in
- Click on _Create Project_

---

# Creating a new R file

- Go to _File_, _New File_, _R Script_
- Add some simple R code, e.g.,
```R
print(2 + 2)
```
- Save and choose a filename ending in .R

---

# Adding the new file to git

- Click on the tab named _git_ (right side)
- Click the _Diff_ button to see an overview of the changes
- Check all changed files to __add__ them to the __staging area__ (could take some time)
- Add a descriptive __commit__ message and click _commit_
- Press close when the commit is done
- Now press __push__ to upload the changes to GitHub
- Fill out your username and password

???
- Altijd eerst een diff doen!
- Username and password worden bewaard ie voor de session, dus dat is wel hip

---

# Advanced/Next steps
- Revert ik heb per ongeluk iets aanpast en het moet weer terug naar hoe het was.
- History is voor te kijken hoe zag iets er eerder uit
- Ignore knop is voor bestanden die je niet online wilt zetten

---

