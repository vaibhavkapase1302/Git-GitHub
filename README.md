# Git-GitHub

<img src="https://github.com/vaibhavkapase1302/Git-GitHub/blob/main/git_and_github_logo.png" width="1300" height="250" alt="Git and GitHub">

- Git is a Distributed Version Control System
- Another Version control system names are SVM, Azure's Git, AWS CodeCommit
- GitHub is a Public Repository

 
## Installing Git
https://git-scm.com/downloads

## Source Code Management

In the DevOps world, everything is treated as code (e.g., code, shell script, configurations, etc.). Robust source code management tools are a must.

* **[Github](https://github.com/)** (Free & Paid): A web-based hosting service for version control using Git. It offers all of the distributed version control and source code management (SCM) functionality of Git as well as adding its own features.
* **[Bitbucket](https://bitbucket.org/)** (Free & Paid): A web-based version control repository hosting service owned by Atlassian, for source code and development projects that use either Mercurial or Git revision control systems.
* **[Gitlab](https://about.gitlab.com/)** (Free & Paid): A web-based DevOps lifecycle tool that provides a Git-repository manager providing wiki, issue-tracking and CI/CD pipeline features, using an open-source license.
* **[AWS CodeCommit](https://aws.amazon.com/codecommit/)** (Free & Paid): A fully-managed source control service that makes it easy for companies hosting their own repositories to collaborate on code in a secure and highly scalable ecosystem.
* **[Azure Repos](https://azure.microsoft.com/en-us/services/devops/repos/)** (Free & Paid): Provides Git repositories or Team Foundation Version Control (TFVC) for source control of your code.
* **[Google Cloud Source Repositories](https://cloud.google.com/source-repositories)** (Free & Paid): Fully-featured, scalable, private Git repositories hosted on Google Cloud.

Git Bash:  Work like Linux cmd
Git CMD: Work like Windows cmd 


# Git Commands:


```sh
git config --global user.name "<your username>"
git config --global user.email "<your email>"
```

Initialise an empty Git Repository

```sh
git init
```

Clone an existing Git Repository 

```sh
git clone <repository URL>
```

Add file/stage to git

```sh
git add <filename>
```

Add all the files to git

```sh
git add .
```

Commit all the staged files to git

```sh
git commit -m "<your commit message>"
```

Restore the file from being modified to Tracked

```sh
git restore <filename>
git checkout <filename>
```

Show the status of your Git respository

```sh
git status
```

Show the branches of your git repository

```sh
git branch
```

Checkout to a new branch

```sh
git checkout -b <branch name>
```

Checkout to an existing branch

```sh
git checkout <branch name>
```

Remove a branch from Git

```sh
git branch -d <branch name>
```

Show remote origin URL

```sh
git remote -v
```

Add remote origin URL

```sh
git remote add origin <your remote git URL>
```

Remove remote origin URL

```sh
git remote remove origin 
```

Fetch all the remote branches

```sh
git fetch
```
Push your local changes to remote branch

```sh
git push origin <branch name>
```

Pull your remote changes to local branch

```sh
git pull origin <branch name>
```

Check you git commits and logs

```sh
git log
```

### Creating SSH Token:

## Create .gitignore 

https://www.toptal.com/developers/gitignore

## All github useful commands:-

```
