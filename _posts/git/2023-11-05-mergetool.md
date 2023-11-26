---
title: "git merge: vim takes you from 'so confusing' to 'so fast'"
categories: 
  - "git"
tags: 
  - "vim"
---

Who really gets git - to say nothing of git merge - now there's your work, someone else's changes, and git in a strange state. (None of which the boss is interested in.) You need to get this all fixed, fast.

Luckily you invested in learning the basic vim editing commands, so you actually have the most powerful tool at your fingertips - it looks complicated at first, but just hold on, it's actually making your life simpler and fast.

The bash commands you need:

git config merge.tool vimdiff
git config merge.conflictstyle diff3
git config mergetool.prompt false
git mergetool

Vim will open in a 4 panel screen like the below:

[![](https://nealcnotes.files.wordpress.com/2023/11/vim-mergetool.png?w=1024)](https://nealcnotes.files.wordpress.com/2023/11/vim-mergetool.png)

You can work through this excellent example if you want to learn it: [https://www.rosipov.com/blog/use-vimdiff-as-git-mergetool/](https://www.rosipov.com/blog/use-vimdiff-as-git-mergetool/)
