---
layout: post
title: "From WordPress to Octopress"
date: 2013-06-02 12:59
comments: true
categories: [programming, miscellaneous, productivity] 
---
{% img center /images/wordpress_to_octopress.png 640 264 'Wordpress to Octopress' %}

## Some changes

You may or may not have noticed that this blog has switched from a
hosted [WordPress](http://www.wordpress.org) blog to a [Octopress](http://octopress.org) blog.
I originally started looking at migrating the blog for a couple of
reasons:

1. I love ruby and I wanted to play around with [Jekyll](http://jekyllrb.com)
2. Jekyll can be deployed easily to [GitHub Pages](http://pages.github.com)
3. Github Pages is free (as in like free beer...) 
4. The amount of comment spam I am getting on WordPress was driving me
   crazy (yes I know I can use Akismet)
5. I wanted to customize my blog a little more than what is allowed
   with WordPress

<!-- more -->
## The initial search

 Initially I started looking at some of the blogging tools that my
friends at the [Hampton Roads Ruby Users Group](http://757rb.org) where using. 
The first one I came across that caught my interest was [Ken Collins'](http://github.com/metaskills) blog: [metaskills.net](http://metaskills.net). 
The metaskills blog uses a modified version of Jekyll which Ken has added in a few items to organize and publish easier.
You can check out his code [here](https://github.com/metaskills/metaskills.net).

### First draft: Jekyll

{% img right /images/octojekyll.png 200 'OctoJekyll' %}
I started out creating a plain Jekyll blog and looking at how the static
site generation worked.
There are plenty of resources on the [Jekyll site](http://jekyllrb.com) which can show you how to install Jekyll and get it running. 
You will need [Ruby](http://www.ruby-lang.org) and
[RubyGems](http://www.rubygems.org). 
If you are dabbling in Ruby or Rails, you will already have both of them.

### Second draft: Jekyll Bootstrap

{% img left /images/Jekyll-bootstrap-screen.png 300 'Jekyll Bootstrap Getting Started screen' %}
While I found Jekyll pretty cool, I wanted my site to have a little bit
of styling.
Not being a graphic designer of any sort, I started looking for some
themes that I could use to modify. 
After doing a little digging on Google for Jekyll themes, I found [Jekyll Bootstrap](http://jekyllbootstrap.com) by
X. Note: There is also another spin off from this project called
[Ruhoh](http://ruhoh.com).

### Final draft: Octopress

{% img right /images/octopress-logo.png 200 'Octopress Logo' %}
I am not sure why I never noticed or found it sooner (as I am sure I
have heard of Octopress before!) -- but I finally stumbled across the
[Octopress site](http://octopress.org). Octopress is a framework
designed by [Brandon Mathis](http://brandonmathis.com) for Jekyll.  

__I had finally found the toolset I was looking for!__ 

Octopress had plenty of themes, still stuck to Jekyll as the method of generating static
sites -- and had plugins which smoothed over some of the 'warts' of
Jekyll out of the box.

Here is some of the static blog-generating goodness (i.e. integrations) you will find in
Octopress:

* Github 
* Google+
* Twitter 
* Disqus 
* Google Analytics
* Pinboard
* Delicious
* Facebook likes

The configuration file in a 'stock' Octopress install is a nice YAML
layout. Here is a snippet:

``` yaml _config.yml
# ----------------------- #
#      Main Configs       #
# ----------------------- #

url: http://yourblogurl.com
title: Your Blog Name
subtitle: Some catchy subtitle..
author: Your Name Here
simple_search: http://google.com/search
description: This will show in the META tags
``` 

Making changes is as easy as changing the appropriate key/value
pair and run ```rake preview``` to view it on http://localhost:4000 

Deploying the site is just as easy:
``` bash
rake generate   #generate the static site content
rake deploy     #deploy the site to your deploy location (i.e. github)
```
You can even abbreviate deployment to: ```rake gen_deploy```

Here is a snippet:

``` yaml Octopress _config.yml file
# ----------------------- #
#      Main Configs       #
# ----------------------- #

url: http://yourblogurl.com
title: Your Blog Name
subtitle: Some catchy subtitle..
author: Your Name Here
simple_search: http://google.com/search
description: This will show in the META tags
``` 

Octopress also has plenty of themes as a starting point for customizing your own blog. 
The github repo [here](https://github.com/imathis/octopress/wiki/3rd-Party-Octopress-Themes) is a good starting point for 3rd party Octopress themes.  

I am now (_for the time being_) sold on Octopress and will be using it for
my posts going forward. If you are in the market for a new static
blogging platform, give it a try -- I think you will be pleasantly
surprised.
