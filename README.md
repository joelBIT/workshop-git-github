# 🛠️ Workshop: Practicing Git & GitHub


## 🏗️ Task 1: The Basics

### 1. Initialize a New Repository
* _git init_
  * Creates a local git repository in the current folder (a .git folder is created in the current folder).
* _git add ._
  * Adds all untracked files and unstaged changes in the current repository to the staging area.
* _git commit -m_ "created styles.css, notes.txt, .gitignore and .env files"
  * The git commit command captures a snapshot of the project's currently staged changes.
* _git branch -M main_
  * Renames branch (from master) to main.

### 2. Connect to GitHub
* _git remote add origin_ https://github.com/joelBIT/workshop-git-github.git
  * Adds a name (origin) for a remote repository (located at the URL).

### 3. Track Changes
* _git status_
  * Shows the working tree status (i.e., which files that are untracked, tracked, modified).
* _git add ._
  * Adds all untracked files and unstaged changes in the current repository to the staging area.
* _git commit -m_ "Updated styles.css with styling for the main element"
  * The git commit command captures a snapshot of the project's currently staged changes.
* _git push -u origin main_
  * Specific way of pushing the new commits to the main branch in the remote repository located at the URL stored in the "origin" variable. The -u parameter means that you push a branch that you have never pushed before.
* _git status_
  * I ran this command again after modifying styles.css and it shows that I modified the styles.css file (unstaged changes).
* _git add_ styles.css
  * I stage the changes I have made to the styles.css file.
* _git commit -m_ "Updated styles.css with styling for the .title class in main"
  * The git commit command captures a snapshot of the project's currently staged changes (styles.css).
* _git push origin main_
  * Specific way of pushing the new commits to the main branch in the remote repository located at the URL stored in the "origin" variable.

### 4. Ignoring Files
* _git add ._ (I have created the .gitignore file and added the .env to its contents)
  * Adds the untracked .gitignore file to the staging area (so it becomes a tracked file, i.e., under version control).
* _git commit -m_ "Created .gitignore"
  * The git commit command captures a snapshot of the project's currently staged changes (.gitignore). Since the .env file is mentioned in the .gitignore file the .env file is not tracked and thus not under version control and not pushed to GitHub.
* _git push_
  * Push the current branch (main) to its remote "tracking branch".


## 🔄 Task 2: Clone, Rename, and Re-Publish
* _git clone_ https://github.com/Lexicon-Smaland/Hello-World.git
  * Creates a local copy of the project
* _git remote show origin_
  * Shows information about the "origin" such as Fetch URL, Push URL and branch.
* _git remote set-url origin_ https://github.com/joelBIT/Hello-World.git
  * Updates the remote URL stored in the "origin" variable to https://github.com/joelBIT/Hello-World.git
* _git status_
  * Shows the working tree status (i.e., which files that are untracked, tracked, modified).
* _git add ._
  * Adds the unstaged changes of the README.md file (I added a comment to the file) to the staging area.
* _git commit -m_ "Added comment o README.md"
  * The git commit command captures a snapshot of the project's currently staged changes (README.md).
* _git push origin main_
  * Pushed the commit to the main branch in the repository located at the URL mapped by "origin", which is https://github.com/joelBIT/Hello-World.git now since I updated "origin" recently.
