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

To revert latest (last one)  change

```sh
git revert HEAD
```


```sh
git log --oneline
```

```sh
git rebase
```

```sh
git chery-pick <hash-value>
```

```sh
git reset --hard HEAD~1
```


### Creating SSH Token:

## Create .gitignore 

https://www.toptal.com/developers/gitignore

## All github useful commands:-


## 🛠️ To Log In to Your Personal GitHub Account Using the CLI, You Typically Use the `gh` CLI (GitHub CLI)

This guide walks you through logging into GitHub via CLI, creating a repository, pushing code, and logging out — all from the terminal.

### 📋 Prerequisites

* ✅ [GitHub CLI (`gh`)](https://cli.github.com/manual/installation)
* ✅ [Git](https://git-scm.com/downloads)
* ✅ A GitHub account (e.g., `vaibhavkapase1302`)


#### **Install GitHub CLI** (if not already installed)

```bash
# macOS
brew install gh

# Ubuntu/Debian
sudo apt install gh

# Windows (via Scoop or Winget)
scoop install gh
```

### 1️⃣ Login to GitHub Using CLI

https://cli.github.com/manual/gh

https://docs.github.com/en/github-cli/github-cli/quickstart

#### 🔸 Command

```bash
gh auth login
```

#### 🔸 Steps

1. Choose: `GitHub.com`
2. Choose: `Login with a web browser`

### ✅ What To Do When You See This

When you run `gh auth login`, you may see this message:

```text
! First copy your one-time code: ABCD-EFGH
- Press Enter to open github.com in your browser...
```

This uses GitHub’s **device authorization flow**.

#### 🔐 Follow these steps:

1. **Copy the one-time code** from the terminal (e.g., `ABCD-EFGH`)
2. **Press Enter** — this opens:

   ```
   https://github.com/login/device
   ```
3. **Paste the code** into the browser page.
4. Log in to your GitHub account (`vaibhavkapase1302`)
5. **Click "Authorize GitHub CLI"** when prompted
6. Go back to the terminal — it should say:

   ```
   ✓ Authentication complete. Logged in as vaibhavkapase1302
   ```

#### ✅ Confirm Login

```bash
gh auth status
```

Expected output:

```
✓ Logged in to github.com as vaibhavkapase1302
```

##3## 2️⃣ Create a New GitHub Repository

```bash
gh repo create hello-world --public --confirm
```

* Use `--private` instead if needed
* Add `--gitignore`, `--license` as needed

#### 3️⃣ Initialize Local Git Project

```bash
mkdir hello-world
cd hello-world
echo "# Hello World" > README.md
git init
git add .
git commit -m "Initial commit"
```

#### 4️⃣ Connect Local Repo to GitHub

#### HTTPS:

```bash
git remote add origin https://github.com/vaibhavkapase1302/hello-world.git
```

#### SSH (if configured):

```bash
git remote add origin git@github.com:vaibhavkapase1302/hello-world.git
```

### 5️⃣ Push Code to GitHub

```bash
git branch -M main
git push -u origin main
```

### ✅ Done!

View your repository:
[https://github.com/vaibhavkapase1302/hello-world](https://github.com/vaibhavkapase1302/hello-world)


### 🧠 Optional: Git Configuration

Set your global Git identity:

```bash
git config --global user.name "Vaibhav Kapase"
git config --global user.email "your-email@example.com"
```

### 🔚 6️⃣ Logout from GitHub CLI

If you want to sign out from GitHub CLI:

#### 🔸 Logout from GitHub.com:

```sh
gh auth logout
```

```bash
gh auth logout --hostname github.com
```

You'll be prompted to confirm:

```
Are you sure you want to log out of github.com? (Y/n)
```

Type `Y` to confirm.

### 🔸 Verify Logout:

```bash
gh auth status
```

Expected output:

```
gh: not logged in to any hosts
```

```txt
brew install gh
gh auth login
gh auth status
gh api user

git init
git add README.md
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/vaibhavkapase1302/ArgoCD-demo.git
git push -u origin main
gh auth logout
gh auth status
gh api user
```

---
