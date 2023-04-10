---
title: "Liftoff - Hugo Apèro"
subtitle: "Building a website with open-source tools"
excerpt: "With much thanks to Dr. Alison Hill and her Hugo Apèro theme, I have created this site. "
date: 2023-04-08
author: "Cathy Holloway"
draft: false
tags:
  - hugo-site
categories:
  - open science
  - R
layout: single
links:
- icon: github
  icon_pack: fas
  name: website
  url: https://github.com/cathyholloway/improbable-professor
- icon: github
  icon_pack: fab
  name: Hugo Apèro 
  url: https://hugo-apero-docs.netlify.app/ 
---

## Why I chose Hugo Apèro

I wanted to build and host a site using open-source tools. I tried a few and failed to love them until I stumbled across the Hugo Apèro theme developed by Dr Alisson Hill. More specifically I found the recording of a workshop to [Introduce yourself online using blogdown and Hugo Apèro workshop tutorial](https://www.youtube.com/watch?v=RksaNh5Ywbo), which i followed.

## What I didn't know 

When I dived head-first into the tutorial, I didn't realise that I would need to have R, RStudio and some packages installed for this to work. Fear not it is easy to install R, then R studio and then add the packages you need. Here is what you do:

1. [install R & R Studio](https://rstudio-education.github.io/hopr/starting.html)
2. [install rmarkdown](https://alexd106.github.io/intro2R/install_rmarkdown.html)
3. Install Hugo (see next tip)

## Tips for installing Hugo
Hugo is a static site builder, and if you have followed along with the tutorial I linked to, you will have seen that, using RStudio, you can connect to GitHub directly. So you edit all your files in RStudio and then push them to Git. And like magic, they appear. However, you still need to build the site where Hugo comes in. Hugo is a static site generator, so it will look into a folder and look for files that have been knitted together in a way it understands. Luckily for you and me, we don't need to know how any of this knitting works. We can just hit the knit button in RStudio, and the magic is done for us, courtesy of Dr Allison Hall. However, your machine needs Hugo installed to knit the right pattern. And it needs the tight version of Hugo for this knitting to work well. So, you need to install Hugo version "0.80.0". The console will give you a prompt for this: 


```console
Error: hugo 0.80.0 not found. You may try blogdown::install_hugo("0.80.0")
```

#### The issue is when you try blogdown::install_hugo("0.80.0"), you get another long error saying it can't be found easily. So you need to find the right version of Hugo and then put it where your computer knows to look for it.

To do this:  
1. Download the right version. [Link to Hugo 0.80.0](https://github.com/gohugoio/hugo/releases/tag/v0.80.0). You will need to scroll to the bottom of this page and then find the version which is suitable for your operating system
2.  Unzip the folder and in there you will find (I am using a MAc and I found) 3 files. A readme a licence and a Hugo exec. It is the Hugo exec you need to copy to somewher your computer knows to find it.
3. Copy Hugo to a place where your computer looks for things. This is in the PATH. You can see where your computer is looking for things by typing the following into a terminal:  echo $PATH. I use the Warp terminal, and there you can see just CMD+click open a file within an output, so I clicked on one place where my computer looks for things and copied the right version of HUGO into this folder, and it all worked out well. 

I then continued with [Introduce yourself online using blogdown and Hugo Apèro workshop tutorial](https://www.youtube.com/watch?v=RksaNh5Ywbo) and started playing, and here we have the result.    I hope this helps. If you have any questions or comments, I'd be happy to try and answer any.
