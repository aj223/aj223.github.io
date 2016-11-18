---
layout: post
title:  "Robots and humans"
date:   2016-11-16 12:19:57 +0000
author: Andrea Johansson
type: article
description: In this blog post I explore robots.txt and humans.txt
image: https://aj223.github.io/assets/postImg.png
---

### robots.txt

The robots.txt file is a file which tells webcrawlers whether they have access
to some of, all of or none of the content on a website. In the file,
user-agents can be defined if the aim is to have different settings for different webcrawlers. 
I have chosen to have the same settings for all webcrawlers, so therefore, the first line in my robots.txt file is:


User-agent: *

Then, it is specified which, if any of the content is disallowed. Here are three different options:

1. Disallow:       (Left blank to allow access to all content. This is what I chose to do). 
2. Disallow: /     (All content is disallowed. This means that the website will not be displayed by search engines).
3. Disallow: /computer.png (This disallows access to a specific file).

I have also chosen to link to my sitemap file for better search engine indexing.

### humans.txt

The humans.txt file is an easy way of adding information about those behind the website. As instructed by [humanstxt.org](http://humanstxt.org/Standard.html), 
I have added information about myself in the humans.txt file and added a link to it in my head file in the includes folder. Having a humans.txt file is by no
means necessary, but makes it easy to prove authorship without putting this information in the actual code.


