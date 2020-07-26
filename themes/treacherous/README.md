# Treacherous - Hugo theme

![I love the vintage movie posters](images/ci-cc72.jpeg "Counter-Espionage")

Treacherous is an ever so slightly hacked fork of the Archie Hugo theme, which remains a minimal and clean theme for hugo with a markdown-ish UI. If you want to base your work off a theme, use that one. You'll be happier.

The Archie theme is, in turn, forked from the [Ezhil Theme](https://github.com/vividvilla/ezhil), which is alsoo pretty clean. My aim was to go for a more brutalist approach, here.

## Demo

[Check the Archie Demo](https://athul.github.io/archie/). I'm not even going to mess with a demo of this one. You can find it working or not working [here](https://treacherous.tech).

## Theme features the following
- Google Analytics Script (not using it)
- Callouts (not using it)
- Tags (Kind of using it)
- Auto Dark Mode(based on system theme, which I'm also not using, don't like dark theme options. It's a subjective thing, I realise.)
- tl:dr; frontamatter (Love this.)

## Installation
In your Hugo website directory, create a new folder named theme and clone the repo
```bash
$ mkdir themes
$ cd themes
$ git clone https://github.com/athul/archie.git
```
Edit the `config.toml` file with `theme="archie"`
For more information read the official [setup guide](https://gohugo.io/overview/installing/) of Hugo.

## Writing Posts
Create a new `.md` file in the *content/posts* folder
```yml
---
title: Title of the post
description:
date:
tldr: (optional)
draft: true/false (optional)
tags: [tag names] (optional)
---
```

## Credits
Forked from [Ezhil Theme](https://github.com/vividvilla/ezhil) and Licensed under MIT License 
Inspired by design of blog.jse.li

----

## Config of the Demo Site

```toml
baseURL = "https://athul.github.io/archie/"
languageCode = "en-us"
title = "Archie"
theme="archie"
copyright = "© Athul"
# Code Highlight
pygmentsstyle = "monokai"
pygmentscodefences = true
pygmentscodefencesguesssyntax = true

paginate=3 # articles per page

[params]
	mode="auto" # color-mode → light,dark or auto
	featherIconsCDN=true
	subtitle = "Minimal and Clean [blog theme for Hugo](https://github.com/athul/archie)"

# Social Tags

[[params.social]]
name = "GitHub"
icon = "github"
url = "https://github.com/athul/archie"

[[params.social]]
name = "Twitter"
icon = "twitter"
url = "https://github.com/athulcajay/"

[[params.social]]
name = "GitLab"
icon = "gitlab"
url = "https://gitlab.com/athul/"

# Main menu Items

[[menu.main]]
name = "Home"
url = "/"
weight = 1

[[menu.main]]
name = "All posts"
url = "/posts"
weight = 2

[[menu.main]]
name = "About"
url = "/about"
weight = 3

[[menu.main]]
name = "Tags"
url = "/tags"
weight = 4
```
