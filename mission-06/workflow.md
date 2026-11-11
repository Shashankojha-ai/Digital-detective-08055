# Mission 6 — Git workflow notes

## Task 6.1 — Status, staging, commit, and history

`git status` reports the current branch and which files are modified, staged, or untracked. `git add` stages selected changes: it prepares a snapshot but does not yet save that snapshot to the repository history. `git commit` records the staged snapshot as a named point in the local history. `git log` shows recent commits so a collaborator can see what has already been recorded.

## Task 6.2 — Branch and README change

The `update-about` branch isolates the learning-notes change from `main`. The root README's `My Learning` section records three things learned so far. The branch is published so GitHub can compare it with `main`.

## Task 6.3 — Pull request

A pull request (PR) proposes changes from one branch to another and provides a place to inspect the diff, discuss it, and request changes before merging. A PR helps collaborators review work without directly changing the target branch. The Mission 6 PR targets `main` and is intentionally left open; it has not been merged.

## Task 6.4 — Git glossary

| Term | One-line explanation |
| --- | --- |
| `init` | `git init` starts a new Git repository in a directory. |
| `status` | `git status` summarizes the current branch and staged or unstaged file changes. |
| `stage` | `git add <file>` selects file changes for the next commit. |
| `commit` | `git commit` records the staged snapshot in local history. |
| `history` | `git log` lists recorded commits. |
| Create/list branch | `git switch -c <name>` creates and switches to a branch; `git branch --list` lists local branches. |
| Switch branch | `git switch <name>` changes the current working branch. |
| Publish | `git push -u origin <branch>` sends a local branch to the remote and sets its upstream. |
| Retrieve remote changes | `git fetch origin` downloads remote references and commits without merging them into the current branch. |
