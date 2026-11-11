# Mission 6 — Version control and collaboration

## Task/objective

Practise Git status, staging, commits, history, branches, and publishing; create a pull request and explain how these tools support collaboration.

## Work completed

- Inspected repository status and recent commit history.
- Staged and committed the Mission 6 notes and evidence.
- Created the requested `update-about` branch from the current published `main`.
- Added a short `My Learning` section to the root README and committed the change on `update-about`.
- Published the branch and opened a pull request targeting `main`; the PR is intentionally left open and unmerged.
- Wrote a one-line glossary for each required Git term.

## Commands/tools used

Git commands used included `status`, `log`, `add`, `commit`, `switch -c`, `push`, `show`, and branch inspection. GitHub CLI was used to open and inspect the pull request. The evidence record gives the sanitized commands and observed results.

## My understanding

Staging selects which file changes will go into the next commit; committing saves that selected snapshot in local history. A branch gives work its own line of development, so it can be prepared without changing `main`. A pull request proposes those changes for review and discussion before merging. Keeping this PR open means it has not been merged into `main`.

## Difficulties faced

The published `main` branch had advanced by one commit after my local checkout was created. That commit removed the Mission 5 converter file.

## How resolved

I inspected the new commit and started `update-about` from the fetched current `main`, preserving the existing remote change rather than overwriting it.

## Evidence/files

- [Git workflow explanations and glossary](workflow.md)
- [Sanitized Git and pull-request evidence](evidence/git-workflow.md)
- The root [`README.md`](../README.md) includes the requested `My Learning` section.

## Commit details

- Mission files commit: `Document Git workflow and terminology`
- Root README commit: `Add Mission 6 learning notes`
- Branch: `update-about`
- Pull request: recorded in the evidence file after creation; the PR is left open and unmerged.