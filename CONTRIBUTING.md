# Contributing to Open-Learning websites

This document covers the process we follow to publish new content on the open-learning websites

- Open-Learning Initiative : [github](https://github.com/open-learninge/open-learning.github.io/) : [web](http://open-learninge.org/)
- Open-Learning Foundation : [github](https://github.com/open-learninge/foundation/) : [web](http://open-learninge.org/foundation/)
- Open-Learning Campus : [github](https://github.com/open-learninge/campus/) : [web](http://open-learninge.org/campus/)

## Fork

Publishing is handled using [GitHub pull-requests](https://help.github.com/articles/using-pull-requests/) from private [fork](https://help.github.com/articles/fork-a-repo/) so first you have to fork this repository.

## Branch

All your changes needed for the post (such as media) has to be contained in the same pull-request. To make things more organized you should contain changes in a separate branch.

## Write

All the websites use [`skinny-bones-jekyll`](https://github.com/mmistakes/skinny-bones-jekyll/) as their engine.

If you are creating a new post there's a [guide](http://mmistakes.github.io/skinny-bones-jekyll/getting-started/#posts) on how to do that.

## Submit

When you have your post completed sent it using a pull-request to the correct repository and branch:

- [`open-learning.github.io`](https://github.com/open-learning/open-learning.github.io/) : `master`
- [`foundation`](https://github.com/open-learning/foundation/) : `gh-pages`
- [`campus`](https://github.com/open-learning/campus/) : `gh-pages`

## Review

Each post should be reviewed by someone in the @open-learning/pr team before getting published.

## Merge

Publishing is completed by [merging your work into the targe branch](https://help.github.com/articles/merging-branches/).

## Sync

If changes were made that should be synchronized between the site we do that with `git cherry-pick`:

> **note**
>
> In this example we asume out remote is called `initiative`, the remote url is `https://github.com/open-learning/open-learning.github.io.git` and the last commit is a merge with all changes we want

```shell
git remote add initiative https://github.com/open-learning/open-learning.github.io.git
git fetch initiative
git cherry-pick -m 1 FETCH_HEAD
```
