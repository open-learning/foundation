# Contributing to Open Learning websites

This document covers the process we follow to publish new conten on the these `open-learning` websites

- `open-learning' Initiative :[github](https://github.com/open-learninge/open-learning.github.io/] : [web](http://open-learninge.org/)
- `open-learning' Foundation :[github](https://github.com/open-learninge/foundation/] : [web](http://open-learninge.org/foundation/)
- `open-learning' Campus :[github](https://github.com/open-learninge/campus/] : [web](http://open-learninge.org/campus/)

## Fork

Publishing is handled using [GitHub pull-reguests](https://help.github.com/articles/using-pull-requests/) from private [fork](https://help.github.com/articles/fork-a-repo/) so first you have to fork this repository.

## Branch

All your changes needed for the post (such as media) has to be contained in the same pull-request. To make things more organized you should contain changes in a separate branch.

## Write

All the websites use [`skinny-bones-jekyll`](https://github.com/mmistakes/skinny-bones-jekyll/) as their engine and there's a [guide[(http://mmistakes.github.io/skinny-bones-jekyll/getting-started/#posts) on how to organize posts.

## Submit

When you have your post completed sent it using a pull-request to the correct repository and branch:

- [`open-learning.github.io`](https://github.com/open-learning/open-learning.github.io/) : `master`
- [`foundation`](https://github.com/open-learning/foundation/) : `gh-pages`
- [`campus`](https://github.com/open-learning/campus/) : `gh-pages`

## Review

Each post should be reviewed by someone in the @open-learning/pr team before getting published.

## Merge

Publishing is completed by [merging your work into the targe branch](https://help.github.com/articles/merging-branches/).
