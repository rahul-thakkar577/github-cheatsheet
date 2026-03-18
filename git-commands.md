# Git Commands Sheet


## Setup and Configuration Command

- git --version
- git config --global user.name "rahul-thakkar577"
- git config --global user.email "rahulthakkar@gmail.com"

- git config
- git config user.name
- git config user.email
- git config --list
Verify configuration
---

## Basic Workflow

- git init
Initialize new Git repo

- git add git-commands.md
Stage file for commit

- git status
check file tracked or untracked

- git commit -m "git-commands.md added"

- git branch -M main
to change branch name

- git remote add origin <url>

- git push -u origin main

# Branching Commands

## git branch
Lists all branches in the repository.

Example:
git branch

---

## git branch <branch-name>
Creates a new branch.

Example:
git branch feature-1

---

## git switch <branch-name>
Switches to another branch.

Example:
git switch feature-1

---

## git switch -c <branch-name>
Creates a new branch and switches to it.

Example:
git switch -c feature-2

---

## git checkout <branch-name>
Switches to another branch (older method).

Example:
git checkout main

---

## git branch -d <branch-name>
Deletes a branch.

Example:
git branch -d feature-2

---

## git push -u origin <branch-name>
Pushes a branch to the remote repository and sets upstream tracking.

Example:
git push -u origin feature-1

---

## git fetch
Downloads changes from remote without merging.

Example:
git fetch origin

---

## git pull
Fetches and merges remote changes into the current branch.

Example:
git pull origin main

---

## git clone
Copies a remote repository to the local machine.

Example:
git clone https://github.com/user/repository.git

# Advanced Git Commands

## git merge
Merges one branch into another.

Example:
git merge feature-login

---

## git merge --squash
Combines all commits into a single commit before merging.

Example:
git merge --squash feature-profile

---

## git rebase
Reapplies commits on top of another branch.

Example:
git rebase main

---

## git log --oneline --graph --all
Shows commit history in graph format.

Example:
git log --oneline --graph --all

---

## git stash
Temporarily saves uncommitted changes.

Example:
git stash

---

## git stash push -m "message"
Stashes changes with a message.

Example:
git stash push -m "work in progress"

---

## git stash list
Lists all stashes.

Example:
git stash list

---

## git stash pop
Applies and removes latest stash.

Example:
git stash pop

---

## git stash apply
Applies stash without removing it.

Example:
git stash apply stash@{0}

---

## git cherry-pick
Applies a specific commit to current branch.

Example:
git cherry-pick <commit-hash>