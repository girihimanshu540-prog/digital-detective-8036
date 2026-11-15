# Mission 6 — Git and GitHub

## 1. Task / objective
Understand version control, stage and commit changes, create a branch,
open a Pull Request, and explain the collaboration workflow.

## 2. Work completed
Branch - Main , update-about

### Task 6.1 — Basic Git workflow

| Git operation | What it does in my own words |
|---------------|------------------------------|
| Check repository status (`git status`) | Shows which files have been changed, which are staged and ready to commit, and which are not tracked by Git yet |
| Stage selected changes (`git add <file>`) | Picks the changes I want to include in the next commit, so I can choose exactly which files get saved |
| Create a commit (`git commit -m "message"`) | Saves the staged changes as a snapshot in the project history, with a message describing what I did |
| View commit history (`git log --oneline`) | Lists the earlier commits, newest first, each with a short ID and its message |

**Difference between staging and committing:** A useful idea is that staging chooses what goes into the next snapshot, and committing actually saves that snapshot.

### Task 6.2 — Branch
(What you did on `update-about` and what you added to the root README.)

### Task 6.3 — Pull Request
(What a branch and a Pull Request are, why they are useful, and the PR
status: merged or not merged.)

### Task 6.4 — Git command glossary

| Operation | One-line explanation |
|-----------|----------------------|
| Initialise a repository (`git init`) | Turns the current folder into a Git repository so Git can start tracking its files |
| Check status (`git status`) | Shows which files are changed, staged or untracked, and which branch I am on |
| Stage changes (`git add <file>`) | Selects the changes I want to include in the next commit |
| Commit changes (`git commit -m "message"`) | Saves the staged changes as a snapshot in the history, with a message describing it |
| View history (`git log --oneline`) | Lists earlier commits, newest first, with a short ID and message |
| Create / list branches (`git branch <name>`, `git branch`) | `git branch <name>` creates a new branch and `git branch` lists all branches, marking the current one with `*` |
| Switch branches (`git switch <name>`) | Moves me to another branch so my files match that branch |
| Publish changes (`git push`) | Uploads my local commits to the repository on GitHub |
| Retrieve remote changes (`git pull`) | Downloads new commits from GitHub and merges them into my current branch (`git fetch` only downloads them without merging) |

## 3. Commands / tools used
All mentioned above .

## 4. My understanding
I understood everything .
