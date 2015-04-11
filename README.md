# Utilities for git filter-branch

These are scripts used to perform part of IPython's Big Split™, and not meant to be a public utility.
The key piece is `clone-whitelist`,
which clones a repo and runs `git filter-branch` to remove the history of files not in a given whitelist.
`git log --follow` is used to track the history across renames within reason.
