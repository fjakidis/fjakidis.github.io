---
layout: post
title:  Git reference
categories: hardware
tags: 
  - Git
  - Github
  - Version Control
---

## Creating or Cloning a Repository
```
git init
git clone <address.git>
```

## Modifying the Repository
```
git add <file>
git commit -m 'description'
git status
git log --oneline
git diff <commit_one> <commit_two>
git branch
```

## Undoing Changes

Remove a staged file from the staging area.

```
git reset HEAD file
```

Revert a file to previous commit

```
git checkout -- <file>
```

Revert repository to a previous commit

```
git reset --hard <previous commit>
```