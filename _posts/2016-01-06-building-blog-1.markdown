---
layout: post
title:  'Building a blog, part 1'
date:   2016-01-11 11:43:42 +0100
---

#Building a blog, part 1 : "Dynamic website" vs. "Flat-file website" vs. "Static website"

I previously explained why I wanted to conquer and settle my own island and the Web ocean. You want to build a blog too? That's great, you may be interested by the notes of what I've learn during my journey... 

Just to precise: I'm not gonna write about service that proposes you to create and host your own blog online, through a nice and user friendly interface **that tries to make you forget that if you can't access your code and content source, you're enslaved**

Instead, let's face a crucial - the real - choice : Dynamic, Flat-file based or static website? Depending on your technical skills and the needs for your website, you may prefer one to another.

## Dynamic website

A dynamic website relies both on a database (SQL most of times) and a applicative server, whatever it runs (Php, Python, etc...) to which the "*dynamic*" refers to. 
Most of the times, we choose to take advantage of these technologies for the use of a CMS (Content Managing System) which comes with a lot of nice features for your blog (supports comments on your posts, multi users edition or even languages choice for the reader)

Among such services :

- Php : WordPress, Drupal, Joomla
- Python : Mezzanine, Django CMS

The installation is also straightforward and it barely requires any technical skill.

## Flat-file based website 
"flat-file" websites commonly refer to dynamic websites that do not rely on databases, but on files instead (one markdown file per post for example)
I'd like to add that this name doesnt' properly justify the distinction, since :
- static websites are also based on Flat-files
- this type of blogs also use a dynamic language to process the requests.
I think the right denomination should be something like "*dynamic f
websites based on flat files*" but whatever, I'm not from marketing. 

The pros and the cons :

**Advantages**: using a application server allows for a lot of features. (comments...  and so on). Plus Flat-file brings a lot of portability and ease of maintenance.

**Drawbacks**: Like in Dynamic website, an application server :
- if you install it by yourself : it brings a lot of complexity to your server and it will use a notable amount of your resources. 
- if you host your blog on an online service : either you have to pay or the service is very poor (I do not personally know a good, reliable hosting service supporting Python or Php... )

## Static websites
Static websites were once dominant in the premise of the Internet. They simply consist of .html .css and .js files that a Web server download to the client. There is no computation made during the request made by the client that simply fetch a file.
Progressively, this simple method faded out during the 90s after the come of richer, more powerful dynamic website. 
However, since a few years, static websites are coming back to take their revenge (!) backed up by *static website builders*. These awesome tools allows a user to write Flat-file on a server (very simple, with a Markdown or Textile format) on **any** Web server!
For code maintenance or even portability it's just heaven <3.

## My choice 
You've got it, don't you? I chose **a static website builder** to launch what you're reading now. Among them, I picked the most famous one, *Jekyll*, also because github offers a service (*github-pages*) that allow you to host a static website computed by Jekyll. Therefore you can simply edit your blog from anywhere (even from your Android phone) as long as you have:

- either an internet connection (and directly edit it on github) 
- or a git client and a text editor (and then push it online when you'll get Internet)

I suggest you to read the next article : Using Jekyll and github-pages. 

It's particularly useful when you want to write your post on your Android phone while not having available network in the transportation... :) 

I'm not gonna write about Jekyll, since a lot of good tutorials already exist out there. Instead I'm gonna write about using Jekyll and github-pages together since all the tutorials I found are either wrong or misleading. I know that seems rough but that's true.
That leads us