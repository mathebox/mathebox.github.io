---
layout: default
title: Git Preferences
permalink: /git/
---

# Git config
{% highlight yaml %}
[color]
    ui = true
[push]
    default = simple
[alias]
    unstage = reset HEAD --
    st = status
    cl = clone
    ci = commit
    co = checkout
    ls = log --pretty=format:"%C(yellow)%h%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate
    ll = log --pretty=format:"%C(yellow)%h%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate --numstat
    d  = diff
    ds = diff --staged
    ca = commit --amend
    au = add -u :/
    f = fetch
    ap = add -p
{% endhighlight %}

# Useful commands & settings

### Automatic prune on fetch and pull
{% highlight plain text %}
git config remote.origin.prune true
{% endhighlight %}

# Resources
- [ProGit](https://git-scm.com/book/)
