# Git Commands Reference

## Setup & Config

### git --version
Shows installed Git version
Example:
git --version

### git config --global user.name
Sets global username
Example:
git config --global user.name "John Doe"

### git config --global user.email
Sets global email
Example:
git config --global user.email "john@email.com"

---

## Basic Workflow

### git init
Initializes a new Git repository
Example:
git init

### git status
Shows current repository state
Example:
git status

### git add
Stages changes for commit
Example:
git add git-commands.md

### git commit
Creates a commit from staged changes
Example:
git commit -m "Add initial Git commands reference"

---

## Viewing Changes

### git log
Shows commit history
Example:
git log

### git log --oneline
Shows compact commit history
Example:
git log --oneline

### git diff
Shows unstaged changes
Example:
git diff

---

## Added Commands

### git rm
This command removes a file from both your computer's folders and the Git "index" (the list of tracked files) in one step.
Example:
git rm old_notes.md

### git mv
This command renames or moves a file while preserving its entire history, automatically staging the change for your next commit.
Example:
git mv readme.md README.md

### git show
Displays the detailed contents and metadata of a specific Git object, such as a commit, tag, or file version.
Example:
git show HEAD:README.md

### git restore
Reverts files in your working directory or staging area to their last committed state.
Example:
If you made a mistake while editing README.md in nano and want to discard those unsaved changes: git restore README.md

---

## Branching Commands

### git branch
Lists all local branches.
Example:
git branch

---

### git branch <branch-name>
Creates a new branch.
Example:
git branch feature-1

---

### git switch <branch-name>
Switches to an existing branch.
Example:
git switch feature-1

---

### git switch -c <branch-name>
Creates and switches to a new branch.
Example:
git switch -c feature-2

---

### git checkout <branch-name>
Old command used to switch branches.
Example:
git checkout feature-1

---

### git checkout -b <branch-name>
Old method to create and switch branch.
Example:
git checkout -b feature-2

---

### git branch -d <branch-name>
Deletes a branch safely.
Example:
git branch -d feature-2

---

### git branch -D <branch-name>
Force deletes a branch.
Example:
git branch -D feature-2

---

## Remote Commands

### git remote -v
Shows configured remote repositories.
Example:
git remote -v

---

### git remote add origin <repo-url>
Adds a remote repository.
Example:
git remote add origin https://github.com/user/repo.git

---

### git push -u origin <branch>
Pushes branch to remote and sets upstream tracking.
Example:
git push -u origin feature-1

---

### git pull origin <branch>
Pulls changes from remote branch.
Example:
git pull origin main

---

### git fetch
Downloads changes from remote without merging.
Example:
git fetch

---

## Clone & Fork Related

### git clone <repo-url>
Creates a local copy of a repository.
Example:
git clone https://github.com/user/repo.git

---

### git remote add upstream <repo-url>
Adds original repository as upstream.
Example:
git remote add upstream https://github.com/original/repo.git

---

---

# Advanced Git – Day 24 Commands

## git merge <branch>
Merges specified branch into current branch.
Example:
git merge feature-login

---

## git merge --squash <branch>
Combines all commits into one before committing.
Example:
git merge --squash feature-profile

---

## git rebase <branch>
Replays commits on top of another branch.
Example:
git rebase main

---

## git rebase --continue
Continues rebase after resolving conflicts.
Example:
git rebase --continue

---

## git log --oneline --graph --all
Shows commit graph visually.
Example:
git log --oneline --graph --all

---

## git stash
Temporarily saves uncommitted changes.
Example:
git stash

---

## git stash push -m "message"
Stashes changes with description.
Example:
git stash push -m "WIP changes"

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

## git stash apply <stash>
Applies specific stash without deleting it.
Example:
git stash apply stash@{1}

---

## git cherry-pick <commit-hash>
Applies specific commit onto current branch.
Example:
git cherry-pick a1b2c3d

---

---

# Undo & Recovery Commands – Day 25

## git reset --soft HEAD~1
Moves HEAD back one commit but keeps changes staged.
Example:
git reset --soft HEAD~1

---

## git reset --mixed HEAD~1
Moves HEAD back and unstages changes (default mode).
Example:
git reset --mixed HEAD~1

---

## git reset --hard HEAD~1
Moves HEAD back and deletes changes from working directory.
Example:
git reset --hard HEAD~1

---

## git revert <commit-hash>
Creates a new commit that undoes a specific commit.
Example:
git revert a1b2c3d

---

## git revert --continue
Continues revert after resolving conflicts.
Example:
git revert --continue

---

## git revert --abort
Cancels an in-progress revert.
Example:
git revert --abort

---

## git reflog
Shows history of HEAD movements (safety recovery tool).
Example:
git reflog
