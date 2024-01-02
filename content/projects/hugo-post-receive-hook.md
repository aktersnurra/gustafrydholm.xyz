---
title: "Hugo Post Receive Hook"
date: 2022-08-16
draft: false
tags: ["git", "hugo"]
---

A shell script for updating a hugo website on a remote server.

```sh
#!/bin/sh

# This hook will update the static website whenever with new commits on each push.

export LC_TYPE="en_US.UTF-8"

www="/var/www"
src="$(pwd)"
name=$(basename "$src" '.git')
web="$www/$name"
dst="$www/git/$name"

[ ! -d dst ] && mkdir -p "$dst"
cd "$dst" || exit 1

stagit "$src"

ln -sf log.html index.html
ln -sf ../style.css style.css
ln -sf ../logo.png logo.png

git --work-tree="$web" --git-dir="$src" checkout -f
cd $web && hugo
```
