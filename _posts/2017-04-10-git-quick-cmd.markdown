---
layout: post
title:  "Git Quick Command"
date:   2017-04-10 10:56:26 -0700
categories: git cmd
---
There are some quick command of git in console mode.

* config
	* git config --global user.name "<Username>"
	* git config --global user.email "<Email address>"
	* git config --global alias.co checkout
	* git config --global core.editor vim
* repository
	* git init
	* git remote add <name> <url>
* commit file
	* git add <filename>
	* git commit -m "comment"
* sync repositiry
	* git clone <repository> <directory>
	* git pull <repository> <refspec>
	* git push
* branch
	* git branch <branchname>
	* git checkout <branchname>
	* git merge <commit>
* tag/log
	* git tag <tagname>
	* git log --decorate
