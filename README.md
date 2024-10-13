
# Git Exercises Summary

This repository contains solutions to 23 Git exercises from [https://gitexercises.fracz.com/](https://gitexercises.fracz.com/). The author has provided detailed explanations and helpful links alongside the solutions. Below is a summary of the exercises, the commands used, and their purposes:

## Exercise 1: master
**Commands:**
- `git start`
- `git verify`

**Purpose:** Verifying basic Git setup and repo initialization.

## Exercise 2: commit-one-file
**Commands:**
- `git add A.txt` or `git add B.txt`
- `git commit -m "add one file"`
- `git verify`

**Purpose:** Demonstrating how to add and commit a file.

## Exercise 3: commit-one-file-staged
**Commands:**
- `git reset HEAD A.txt` or `git reset HEAD B.txt`
- `git commit -m "destage one file"`
- `git verify`

**Purpose:** Removing a staged file before committing.

## Exercise 4: ignore-them
**Commands:**
- Editing `.gitignore` file (e.g., adding `*.exe`, `*.o`)
- `git add .`
- `git commit -m "commit useful files"`
- `git verify`

**Purpose:** Ignoring files from Git tracking using `.gitignore`.

## Exercise 5: chase-branch
**Commands:**
- `git checkout chase-branch`
- `git merge escaped`
- `git verify`

**Purpose:** Merging branches in Git.

## Exercise 6: merge-conflict
**Commands:**
- `git checkout merge-conflict`
- `git merge another-piece-of-work`
- Edit and resolve conflict, then commit

**Purpose:** Resolving merge conflicts.

## Exercise 7: save-your-work
**Commands:**
- `git stash` or `git stash push`
- Modify files and commit
- `git stash apply`

**Purpose:** Using stashes to temporarily save changes.

## Exercise 8: change-branch-history
**Commands:**
- `git checkout change-branch-history`
- `git rebase hot-bugfix`
- `git verify`

**Purpose:** Rebasing a branch to change history.

## Exercise 9: remove-ignored
**Commands:**
- `git rm --cached ignored.txt`
- `git commit -am "untrack ignored.txt"`
- `git verify`

**Purpose:** Untracking files that are added to `.gitignore`.

## Exercise 10: case-sensitive-filename
**Commands:**
- `git reset HEAD^`
- `mv File.txt file.txt`
- `git add file.txt`
- `git commit -m "lowercase filename"`
- `git verify`

**Purpose:** Handling case-sensitive filenames.

## Exercise 11: fix-typo
**Commands:**
- Fix a typo, then `git commit -a --amend`
- `git verify`

**Purpose:** Correcting typos in commits using `--amend`.

## Exercise 12: forge-date
**Command:**
- `git commit --amend --no-edit --date="1987-08-03"`

**Purpose:** Faking commit dates.

## Exercise 13: fix-old-typo
**Commands:**
- `git rebase -i HEAD^^`
- Edit commits, resolve conflicts, and rebase.

**Purpose:** Fixing old typos by rebasing and editing commits.

## Exercise 14: commit-lost
**Commands:**
- `git reflog`
- `git reset --hard HEAD@{1}`
- `git verify`

**Purpose:** Recovering lost commits using `git reflog`.

## Exercise 15: split-commit
**Commands:**
- `git reset HEAD^`
- Commit files separately with individual messages.

**Purpose:** Splitting one commit into multiple commits.

## Exercise 16: too-many-commits
**Commands:**
- `git rebase -i HEAD~4`
- Use `squash` to merge commits.

**Purpose:** Squashing multiple commits into one.

## Exercise 17: executable
**Commands:**
- `git update-index --chmod=+x script.sh`
- `git commit -m "make executable"`
- `git verify`

**Purpose:** Making files executable in Git.

## Exercise 18: commit-parts
**Commands:**
- `git add --patch file.txt`
- Split and stage hunks with various options (e.g., `y`, `n`, `s`).

**Purpose:** Adding parts of files to commits interactively.

## Exercise 19: pick-your-features
**Commands:**
- `git log --oneline --decorate --graph --all`
- `git cherry-pick` specific commits or SHA-1 hashes.

**Purpose:** Selecting features (commits) from other branches.

## Exercise 20: rebase-complex
**Command:**
- `git rebase --onto your-master issue-555 rebase-complex`

**Purpose:** Advanced rebasing to rearrange commit history.

## Exercise 21: invalid-order
**Command:**
- `git rebase -i HEAD~4` to reorder commits.

**Purpose:** Reordering commit history.

## Exercise 22: find-swearwords
**Commands:**
- `git log -S shit`
- `git rebase -i HEAD~105` and fix the commits with offensive words.

**Purpose:** Finding and replacing inappropriate language in past commits.

## Exercise 23: find-bug
**Two Methods:**
1. Using `git bisect`
2. Using `gitpython` (Python library to automate Git operations).

**Purpose:** Finding bugs using `git bisect` and automating the process with Python.

Each exercise teaches important Git commands like `git add`, `commit`, `merge`, `reset`, `rebase`, `cherry-pick`, `bisect`, and others, while also emphasizing practical applications like resolving conflicts, managing commit history, and automating tasks with Git libraries.
