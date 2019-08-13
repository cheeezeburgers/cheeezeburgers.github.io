---
header:
  teaser: /assets/images/header-default.jpg
  image: /assets/images/header-default.jpg
  overlay_image: /assets/images/header-default.jpg
  overlay_filter: 0.2 # same as adding an opacity of 0.5 to a black background
  caption: "Photo by Iqbal Muakhid on Unsplash"
  actions:
  - label: "More Info"
    url: "https://unsplash.com"
title: "Jekyll & mm Documentation"
categories:
  - Documentation
tags:
  - docs
  - documentation
  - jekyll
  - mm
  - theme
toc: true
toc_label: "  Index"
toc_icon: #"cog"
---

This is my own documentation of Jekyll serve and mm Theme.

## Index

> *siehe rechts >*

## Deployment

run `bundle exec jekyll serve`

> `jekyll serve` **will not work!**

## Post format

### Post Header

```yml
header:
  teaser: /assets/images/header-default.jpg
  image: /assets/images/header-default.jpg          # ODER overlay
  overlay_image: /assets/images/header-default.jpg
  overlay_filter: 0.2 # same as adding an opacity of x.x to a black background
  caption: "Photo by Iqbal Muakhid on Unsplash"
  actions:
  - label: "More Info" # "Download" ...
    url: "https://unsplash.com"
```

### Title & Subtitle

```yml
title: "Jekyll & mm Documentation"
subtitle: "Version 2.0"
description: "A flexible Jekyll theme for your blog or site with a minimalist aesthetic."
```

# Date and Teaser

```yml
date:           # to repost. syntax: 2019-04-18T15:34:30-04:00
excerpt_separator: "<!--more-->"
```

### Meta (cat & tag)

```yml
categories:
  - Documentation
tags:
  - docs
  - documentation
  - jekyll
  - mm
  - theme
```

### Author

```yml
name: "Michael Rose"        # overwrite author
```

### TOC

```yml
toc: true
toc_label: "  Index"
toc_icon: #"cog"
```

## Page format

```yml
---
layout: posts
permalink: /404.html
title: "Page Not Found"
excerpt: "Page not found. Your pixels are in another canvas."
sitemap: false      # not in menu
author_profile: true
link: https://github.com   # posting a link
---
```

## Troubleshooting

+ https://jekyllrb.com/docs/step-by-step/01-setup/
  + official docs (shitty)
+ https://github.com/jekyll/jekyll/issues/3103
  + gem 'github.pages' error
    + > `jekyll serve` **will not work!**
    + run `bundle exec jekyll serve`
