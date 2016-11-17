---
layout: post
title:  "Pre-compiling CSS"
date:   2016-11-14 16:19:57 +0000
author: andreajohansson
type: article
description: In this blog post I discuss the advantages and disadvantages of using SCSS over CSS and describe which SCSS techniques were used in creating this website.
---
Previously, I have only made websites using HTML and CSS. 
I tend to use an online colour scheme generator such as [Coolors](https://coolors.co/) in order to choose a few colours that complement each other nicely to use on the website.
Finding a combination of colours that is user friendly as well as aesthetically pleasing is usually a case of trial and error, so with CSS I have to go in and change the colour code everywhere the particular colour is used. This takes a while to do and mistakes are easily made.

With pre-compiled CSS in the form of SCSS, this problem was eliminated. I simply declared a number of variables and assigned a colour code to each, and when setting the colour of a particular element, 
I used the variable of the colour I wanted, e.g. $navBtn instead of #CC8A8D. Another useful feature of SCSS is that it allows for functions to be used. I wanted my navigation buttons to get darker when hovered over, so I used the function darken($navBtn, 20%) to achieve this.

SCSS also allows for nesting, which makes the code more readable. 
Rather than listing nav, nav ul, nav ul li and so on separately, the sub-elements can be listed inside the curly brackets of nav. This has made it easier for me to see which code I am meant to change.

So far, based on my own experience, I can mainly think of pros of pre-compiling CSS using SCSS, but there can be problems. 
Even though SCSS shares a lot of features with CSS, it is a new language and takes some learning. This could be a problem if you work in a team where some members have little experience of pre-compiling CSS or have used another CSS pre-processor in the past.

Initally, I had some problems with working out a folder structure that led to the SCSS in my source directory being converted to a corresponding CSS file in my _site directory. This problem, or other potential problems occurring while converting from SCSS to CSS is a complication you can avoid by only using CSS.

Still, I have so far found that using a CSS pre-processor such as SCSS leads to cleaner code with fewer mistakes and is more time efficient.
