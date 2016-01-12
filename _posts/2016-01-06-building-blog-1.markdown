---
layout: post
title:  'Building a blog, part 1 : "Dynamic website" vs. "Flat-file website" vs. "Static website"'
date:   2016-01-11 11:43:42 +0100
---

You want to settle your own island and the Web ocean? Fine, it's your choice. But here we're gonna explain the second choice you'll have to face, taking into consideration your technical skills level and the needs for your website.

## Dynamic website

A dynamic website commonly refers to a one that relies both on a database (SQL most of times) and a applicative server, whatever it runs (Php, Python, etc...) 
This technologies allow for the use of a CMS (Content Managing System) which comes with a lot of nice features for the blog (supports comments on your posts, multi users edition or even languages choice for the reader)

Among such services :

- Php : WordPress, Drupal, Joomla
- Python : Mezzanine, Django CMS

The installation is also straightforward and it rarely requires any technical skill.

## Flat-file based website 
Technically, a static website is also based on Flat-files but when it comes to marketing, a "flat-file" website commonly refers to a dynamic website that do not rely on a database, but on file instead (one markdown file per post for example)

Advantage: using a application server allows for a lot of features. Flat-file brings a lot of portability and ease of maintenance. 
Drawbacks: Like in Dynamic website, an application server :
- if you install it by yourself : it brings a lot of complexity to your server and it will use a notable amount of your resources. 
- if you host your blog on an online service : either you have to pay or the service is very poor (I do not personally know a good, reliable hosting service supporting Python or Php... )

## Static websites
Static websites were once dominant in the premise of the Internet. It's simply .html .css and .js files that a Web server provides to the client. There is no computation made during the request for a client that simply fetch a file.
Then this simple method progressively faded out during the 90s with the come of richer, more powerful dynamic website. 
However since a few years static websites are coming back to take their revenge (!) backed up by *static website builders*. These awesome tools allows a user to write Flat-file on a server (very simple, with a Markdown or Textile format)
