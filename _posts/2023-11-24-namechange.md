---
layout: post
author: Neal C
title: Author name wrong in Git repo?
date: 2023-06-18
categories: [git]
tags: [rebase, rename]
---

The name is wrong, or we need to change it, fast.
To fix the Author Name etc on all commits in a github repo, an easy way is

{% highlight bash linenos %}
git rebase -r --root --exec "git commit --amend --no-edit --reset-author"
git push -f
{% endhighlight %}

Read more at https://stackoverflow.com/a/1320317
