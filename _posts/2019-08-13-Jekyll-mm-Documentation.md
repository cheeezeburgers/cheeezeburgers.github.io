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

- [Index](#index)
- [Deployment](#deployment)
- [Post format](#post-format)
- [Page format](#page-format)
- [Troubleshooting](#troubleshooting)

## Deployment

run `bundle exec jekyll serve`

> `jekyll serve` **will not work!**

## Post format

```yml
---
title: ""
categories:
  - CAT
tags:
  - TAG
# additional
#date:           # to repost. syntax: 2019-04-18T15:34:30-04:00
#excerpt_separator: "<!--more-->"
#link: https://github.com   # posting a link
---
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
---
```

## Troubleshooting

+ https://jekyllrb.com/docs/step-by-step/01-setup/
  + official docs (shitty)
+ https://github.com/jekyll/jekyll/issues/3103
  + gem 'github.pages' error
    + > `jekyll serve` **will not work!**
    + run `bundle exec jekyll serve`
