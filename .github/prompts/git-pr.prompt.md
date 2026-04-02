---
agent: 'agent'
model: Claude Haiku 4.5
description: 'Create PR from current branch'
---
Create PR from all changes on current branch.

* Analyse the changed files on the current branch to determine why/what has been changed.
* Create a PR containing clear details of the changes that have been implemented.
* The PR should include a brief summary highlighting the changes and a clear reason why they are being implemented.
* PR comments should be written to a temporary markdown file before submission, ideally in /tmp directory.
* PR comments should be applied using the --body-file syntax.
* The temporary markdown files can be removed once complete.
* If the current branch already has a PR, update any comments accordingly.