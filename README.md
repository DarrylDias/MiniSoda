MiniSoda
========

A blogging framework build on top on Jekyll.

#### Features

* Github Flavored Markdown
* SASS
* Liquid templating
* Built-in sitemap generator

### Setup

**Installing**

``` bash
sudo gem install bundler 
bundle install
```


**Generating static blog files.**

``` bash
rake build
```

**Starting Server**

``` bash
rake server
```

MiniSoda uses the following string in its front-matter

``` md
---
layout: post
title:  
date:   
categories:
comments:
description:
---
```

MiniSoda is in development stage and may contain bugs. If you would like to contribute feel free. Report a bug [here](https://github.com/DarrylDias/MiniSoda/issues)
