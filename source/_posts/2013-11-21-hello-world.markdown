---
layout: post
title: "Hello World"
date: 2013-11-21 13:43:28 +0700
comments: true
categories:
---

Starting to blog with octopress! blogging with markdown is fun!

First time push, github pages not showing my blogs content. Trying again

## Steps on blogging with Octopress 

(So I don't always google)

<!-- more -->

Notes copied from [octopress docs](http://octopress.org/docs/blogging/)

### New article

```
rake new_post["This is awesome article title!"]
```
edit headers, add categories. Example:
```
# One category
categories: Code
 
# Multiple categories example 1
categories: [Code, C++]
 
# Multiple categories example 2
categories:
- Code
- C++
```

### New Pages

```
rake new_page[super-awesome]
# creates /source/super-awesome/index.markdown
```

### Content

Inserting `<!-- more -->` will prevent the post content below this mark from being displayed on the index page for the blog posts

### Generate, Preview, Publish

```
bundle exec rake generate   # Generates posts and pages into the public directory
bundle exec rake preview    # Watches, and mounts a webserver at http://localhost:4000
bundle exec rake deploy     # Deploy to git
```