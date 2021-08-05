---
title: "Set-up"
description: "For Hugo and GH pages setup"
background: 
date: "2019-12-11"
---

### Haven't been able to replicate, good luck.

    hugo new site quickstart  
    cd quickstart  
    git init  
    git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke  

#### Change config toml:

    baseURL = "https://example.org/"
    languageCode = "en-us"
    title = "My New Hugo Site"
    theme = "ananke"

#### Commands to get on Github pages

    cd public && git add --all && git commit -m "Publishing to gh-pages" && cd ..
    git worktree add -B gh-pages public upstream/gh-pages
    $ git worktree add -B gh-pages public origin/gh-pages
    git push upstream gh-pages
    git push origin gh-pages
    git push Facet gh-pages

#### To use html, add line to config.toml

    [markup.goldmark.renderer]
    unsafe = true

#### Example html:

    <div style="text-align: right;">"