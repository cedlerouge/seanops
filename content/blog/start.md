+++
author = "cedlerouge"
categories = ["other"]
date = "2018-12-24"
description = "how it began"
title = "Start"
type = "post"
+++

In this post, I explain how can I deploy this website. The goal is to have a mechanism if CI/CD. 
I use hugo framework for manage localy content and push it in a github repository. 

I follow this (Artem Sidorenko's article)[https://www.sidorenko.io/post/2018/12/hugo-on-github-pages-with-travis-ci/] 
which was very useful when you want to use (travis-ci)[https://travis-ci.com] as a pipeline worker. 

Here were the steps: 
1. Install hugo on your personnal workspace
```bash
$ sudo apt-get install hugo 
```
2. Create the local repository environment
```bash
$ mkdir dev/website
$ cd dev/website
$ git init
$ echo "# My super new website" > README.md
$ git add README.md
$ git commit -m "feat: first commit"
```
3. Create two repositories in github. One for the hugo website files and the other one is for the public static content file. 

I use hugo to help me manage the content. 
I use github to host my site.
I use travis to continuous deliver the content of my notes.

