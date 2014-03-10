---
layout: post
title:  "Rules to live by (and with)."
date:   2014-03-10 13:33:00
categories: jekyll
published: true
---

## Rules.module. Can't live with it. Can't live without it.

So I really can't stand [Rules.module](http://drupal.org/project/rules/). It's an abstraction of an abstraction. The time spent teaching how to use Rules UI and shown how to build a rule, test the rule, export a rule, and debug a rule could easily be spent teaching someone how to code.

I don't have time to go into the details of how much more complex Rules makes Drupal right now, but I will soon.

At the same time, you can't seem to avoid rules.module. Most sites I come across have it.  Drupal Commerce is built on Rules module.

### Hooks are where it's at.  Code can be so simple.  

It just hit me how to deal with this. In Drupal 8, we should build a rules_generator.module.  This module would turn the Rules you've created into actual, readable code using standard Drupal hooks.  Symfony uses generators all the time. Twig is generated.  If we could export Rules into *actual* code, we could turn off rules module entirely once we've generated our site's own custom module.

This could be automatic and cached, or it could be copied out and modified, living on as it's own module.

This is just an idea, I just decided to get it out as fast as I could, remembering I've got a new blog to play with.

Thoughts?
