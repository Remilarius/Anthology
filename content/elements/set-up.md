---
title: "Set-up"
description: "For Hugo and GH pages setup"
background: 
date: "2019-12-11"
---
```html
hugo new site quickstart  
cd quickstart  
git init  
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke  
```
Change config toml:
```html
baseURL = "https://example.org/"
languageCode = "en-us"
title = "My New Hugo Site"
theme = "ananke"
```