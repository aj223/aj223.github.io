---
layout: post
title:  "Comments and social media sharing"
date:   2016-11-17 12:19:57 +0000
author: Andrea Johansson
type: article
description: In this blog post I talk about how I have enabled for comments on blog posts and how Open Graph is used.
image: https://aj223.github.io/assets/postImg.png
---

Today, social media is one of the most powerful tools of communication for socialising as well as businesses
and news outlets. A blog, such as this one, needs to have means of the reader to communicate 
with the writer(s) as well as other readers in order to count as social media and not just media.

That is why I have enabled comments on this blog. Since Jekyll has no native support for comments, 
I have chosen to use [Disqus](https://disqus.com). I wanted comments to appear in blog posts only, so therefore
I pasted the Disqus code in my layout file for posts, but not in my other layout files. This way, comments will be 
automatically enabled under all new posts I create, but there is still the option to disable comments for specific posts.

Social media sharing is today one of the easiest ways of reaching a wider audience, as, for example,
a Facebook post containing a link to a website is liked or shared and thereby spreading to more people. 
In order to maximise the benefits of social media sharing, it is important that the website's meta tags
are set up in a way that means that the social media platform can find key information, such as a title and a description
and put this in the post so that whoever sees the post gets a sense of what the link is about. Having an image appear is
another way of catching the attention of the reader. 

An easy way of achieving this when developing a website is to use Open Graph meta tags. I have chosen to create a file for the content 
I want in the head part of each HTML page in my includes folder. That way, it can easily be imported to all pages, and if changes are made,
they will be applied everywhere. The Open Graph tags, such as _og:title_ and _og:description_ are set to have the content of the title and description of 
the specific page they are on. The title and description are defined in the Front Matter of every page, along with other kinds of information about the page.

Since Open Graph tags are now found on every page, as long as the content is defined for that page, social media platforms such as Facebook will search for these tags
and use the content when forming the post created when a link is shared. This should raise the chances of wider exposure of the website on social media.
