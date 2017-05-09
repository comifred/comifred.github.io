---
layout: post
title:  "Comparation of Git and SVN commands"
date:   2017-05-08 10:06:16 -0700
categories: git cmd
---

There are many users switch from SVN to Git. And there are common questions about which is the command in Git mapping to the one in SVN?  
Some typical mappings will be listed here.  
  
It is worth to note that Git works in peer-to-peer mode, while SVN works in client-to-server mode.  
So not every command in SVN has the exactly same meaning with its counterpart in Git.  

| SVN                                          |---| Git                     |
| -------------------------------------------- |---| ----------------------- |
| svnadmin create *repo*                       |   | git init                |
| svn import *path* *file://repo*              |   | git add .               |
| svn checkout *url*                           |   | git clone *url*         |
| svn checkout -r *rev*                        |   | git checkout *rev*      |
| svn update                                   |   | git pull                |
| svn status                                   |   | git status              |
| svn diff                                     |   | git diff                |
| svn diff -r*rev* path                        |   | git diff *rev* path     |
| svn add *file*                               |   | git add *file*          |
| svn rm *file*                                |   | git rm *file*           |
| svn mv *file*                                |   | git mv *file*           |
| svn commit                                   |   | git commit -a           |
| svn log                                      |   | git log                 |
| svn blame *file*                             |   | git blame *file*        |
| svn copy *trunk-url* *branch-url*            |   | git branch *branch*     |
| svn switch *branch-url*                      |   | git checkout *branch*   |
| svn list *branches*                          |   | git branch              |
| svn copy *trunk-url* *tag-url*               |   | git tag -a *name*       |
| svn list *tags*                              |   | git tag -l              |
| svn merge -r *created-rev*:HEAD *branch-url* |   | git merge *branch*      |
| svn merge -c *rev* *branch-url*              |   | git cherry-pick *rev*   |
| svn switch *branch-url*                      |   | git checkout --track -b *branch* origin/*branch* |
| patch -p0 *patch-file*                       |   | git apply *patch-file*  |

