---
layout: post
title: "Testing org-mode Features"
date: 2014-09-22 11:18:32 -0500
comments: true
categories: Emacs Testing chill
---
* Let's test out some basic org ... stuff.

  I'm not using org-octopress for this post, havent took the time to look through the code and figure
out exactly what that mode is *doing*. So this post is just sort of a test to see how default orgmode
is going to render. I find myself constantly doing these types of redundant tests, it may seem silly 
but it helps me to learn and understand new things, so ... /chill/.

 
** (Re)Review
   
   We've already seen some basics but that was using org-octopress.el, so we might as well go through
it all again... Watch none of this work and this whole post just comes out as garbage....

*Some bold text*
/Some italisized text/ 
_Some underlined text_
+Some strikethough text+
=Some code text=
~Some verbatim text~     - Same thing??

* Ok, now just a table and maybe a couple misc objects

** Make a table out of a random ls's output.
   Blah..

     |-------------+---------+-------------+------------|          
     |         107 | Sep  14 |       06:40 | New.org~   |
     |        9393 | Sep  14 |       09:01 | New.html~  |
     |        8711 | Sep  14 |       09:08 | New.html   |
     |         984 | Sep  14 |       09:08 | New.org    |
     |          89 | Sep  14 |       10:50 | Todo.org~  |
     |       11288 | Sep  14 |       11:13 | Todo.html~ |
     |       16897 | Sep  14 |       12:10 | Todo.html  |
     |        1954 | Sep  14 |       12:10 | Todo.org   |
     |         117 | Sep  15 |       00:06 | index.org~ |
     |-------------+---------+-------------+------------|
     | 49540 Bytes | Stuff   | 19:07 Hours | 9 Files    |



** This will probably be ugly and possibly kill the whole thing..
   Wiiiide table
  |------+------------------------------+---------------------+--------------------+------------------------+------------------------|
  | Edit | [[file:~/.emacs::(require%20'command-log-mode)][.emacs]]                       | [[file:~/Org]]          | [[file:~/.emacs.d]]    | [[file:~/.emacs.d/themes]] | [[file:~/.emacs.d/Vendor]] |
  | Sys  | file:~/.zshrc                | file:~/.bashrc      | file:~/.zprofile   | file:~/.profile        | file:~/.xinitrc        |
  | Org  | file:~/Org/FrequentFiles.org | file:~/Org/Todo.org | file:~/Org/New.org | file:~/Org/Notes.org   | file:~/Org/Blog.org    |
  |------+------------------------------+---------------------+--------------------+------------------------+------------------------|


Hmm, I wonder what a time stamp will look like.. <2014-09-22 Mon>
Now maybe and "inactive" time stamp..  [2014-09-22 Mon]
Also, TODO's:
* TODO Apparently you HAVE to start all Headlines at the *first* column, Like WTF?
- [ ] Sucky
- [ ] Shity
- [X] Sorry
- [ ] Slobering
- [ ] Soviets

* TODO : Kill all Seven Shity Slobering Sucky Sorry Slow-ass Soviets.


* Oh.. I dunno..

** A little list with org links
   Hmmm...
*** Frequently Edited Files

- [[file:~/.emacs]]
- [[file:~/.i3/config]]
- [[file:~/.zshrc::plugins%3D(github%20colored-man%20emacs)][zshrc]]
- [[file:~/.zprofile]]
- [[file:~/i3.conkyrc::TEXT][i3.conkyrc]]
- [[file:~/.bashrc::alias%20Running%3D'echo%20Seeing%20if%20@1%20is%20rUnNninG...%20&%20ps%20-A%20|%20grep'][bashrc]]
- [[file:Todo.org::*My%20app%20in%20PC%20SCHEDULED:%20<2014-11-06%20Thu%2009:15>][FrequentFiles.org]]


* Ok, that was so much fun

  Let's see if it was all just a waste of time and we just created a big dump of garbage..

-EOP-
