+++
draft = false
title = "Revert Git Commits"
date = 2019-01-07T22:44:18-05:00
slug = "revert-git-commits" 
tags = ["git"]
categories = []
+++

# Revert Git Commits

Let's keep this first simple by focusing on a simple, yet helpful, git change.
Sometimes mistakes are made and commits need to be reverted. There are two
options depending on whether the commit has been pushed or not.

## Commit not pushed

`git reset HEAD~1`

## Commit pushed

* `git reset --hard <desired_commit> (eg. 57f05fgds)`
* `git reset --soft HEAD@{1}`
* `git commit -m "Revert to 57f05fgds"`
