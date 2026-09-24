# 🛠️ Workshop: Practicing Git & GitHub


## 🏗️ Task 1: The Basics

### 1. Initialize a New Repository
* git init
  * Creates a local git repository in the current folder (a .git folder is created in the current folder).
* git add .
  * Adds all untracked files and unstaged changes in the current repository to the staging area.
* git commit -m "created styles.css, notes.txt, .gitignore and .env files"
  * The git commit command captures a snapshot of the project's currently staged changes.
* git branch -M main
  * Renames branch (from master) to main.

### 2. Connect to GitHub
* git remote add origin https://github.com/joelBIT/workshop-git-github.git
  * Adds a name (origin) for a remote repository (located at the URL).

### 3. Track Changes
* git status
  * Shows the working tree status (i.e., which files that are untracked, tracked, modified).
* git add .
  * Adds all untracked files and unstaged changes in the current repository to the staging area.
* git commit -m "Updated styles.css with styling for the main element"
  * The git commit command captures a snapshot of the project's currently staged changes.
* git push -u origin main
  * Specific way of pushing the new commits to the main branch in the remote repository located at the URL stored in the "origin" variable. The -u parameter means that you push a branch that you have never pushed before.
* git status
  * I ran this command again after modifying styles.css and it shows that I modified the styles.css file (unstaged changes).
* git add styles.css
  * I stage the changes I have made to the styles.css file.
* git commit -m "Updated styles.css with styling for the .title class in main"
  * The git commit command captures a snapshot of the project's currently staged changes (styles.css).
* git push origin main
  * Push the current branch (main) to its remote "tracking branch".

### 4. Ignoring Files
* git add . (I have created the .gitignore file and added the .env to its contents)
  * Adds the untracked .gitignore file to the staging area (so it becomes a tracked file, i.e., under version control).
* git commit -m "Created .gitignore"
  * The git commit command captures a snapshot of the project's currently staged changes (.gitignore). Since the .env file is mentioned in the .gitignore file the .env file is not tracked and thus not under version control and not pushed to GitHub.
* git push
  * Push the current branch (main) to its remote "tracking branch".


## 🔄 Task 2: Clone, Rename, and Re-Publish

