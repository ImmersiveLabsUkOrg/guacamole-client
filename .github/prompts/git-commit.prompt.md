---
agent: 'agent'
model: Claude Haiku 4.5
description: 'Commit All Changed Files'
---
Stage and Commit all changed files on current branch.

* Never attempt to commit files directly to either the "main" or "master" branches.
* If the current branch is "main" or "master", create a new branch named in accordance with the technical changes.
* All files should be staged, then committed with brief but accurate comments.
* Comments should reflect the business logic of the change.
* Run pre-commit only on files changed in this commit
* Files updated by pre-commit hooks must be accounted for and staged accordingly.
* Commit only when all changed files have been staged.
* Push/Publish the branch if not already done.