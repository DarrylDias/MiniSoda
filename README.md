MiniSoda
========

A blogging framework for artisan

#### Features

* Github Flavored Markdown
* SASS
* Liquid templating
* Built-in sitemap generator
* Works with any Jekyll theme
* Easy embeding of Gist.
* Clean syntax highlighting

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

``` yaml
---
layout: post
title:  
date:   
categories:
comments:
description:
keywords:
---
```

MiniSoda is in development stage and may contain bugs. If you would like to contribute feel free. Report a bug [here](https://github.com/DarrylDias/MiniSoda/issues)
