---
layout: post
title: "What every developer needs to know about certificates"
date: "2021-03-03 23:42:07 +0100"
---
# Backstory

## Will I ever need to deal with that stuff?

As a beginner softwarer developer you probably don't care much about
certificates, private keys and other things related to security of your apps.
You just stick to good old HTTP, make sure you didn't forget to paste all of
these weird `--insecure --notls --yesiwantthisfreebitcoin` flags, skip all
warnings...  

Your main goal is just to make things work, and in this early stage **there's
nothing wrong with that**!

Then, as time passes, you start to feel that you know your favorite language in
and out. You develop project after project — thanks to the framework you picked
up. You know all the tools that might come handy when building your
appplication. And you finally got there — you've got your first junior position.

## Nothing can break the spell, right?
All of a sudden, the part that was completely out of your interest is back
with a vengeance — **security**.

Hell breaks loose. Your brain desperately tries to get through all of these
error messages, documentation pages and StackOverflow answers. And all of these
have something in common — they are filled with some mysterious acronyms like
**SSL, TLS, CA, X.509, CSR, RSA**...

– I bet you had to dive into some really advanced topic to have to deal with all
that stuff.  
– **Not at all**. In fact, if you're unprepared, you may face these problems
really soon.

## You see, let's assume that...

**...communication between your apps must be *encrypted*, so you've been told to
generate some *certificates*.**

*That's no problem! In fact, I've already generated hundreds of them on my Udemy
account, just in case!*

**...your teammate apparently has a problem with that huge *"Your connection is
not private"* message being your new landing page.**

*Man, how did you not know that!? Look, you just click on Advanced, then at
the bottom there's...*

**...your team's artifact repository uses a *self-signed* certificate.**

`What?`  
`Your FAVORITE-PACKAGE-MANAGER is evolving!`  
`Congratulations! Your FAVORITE-PACKAGE-MANAGER evolved into
FANCY-ERROR-PRINTER!`

*Okay, now it's kind of a problem...*

Without at least basic knowledge of common-used authentication mechanisms one
can get really confused when moving to professional working environment. Let's
explain these mechanisms and make all the related terminology a little clearer.
