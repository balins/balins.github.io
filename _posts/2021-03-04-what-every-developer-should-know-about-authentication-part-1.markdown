---
layout: post
title: "What every developer should know about authentication (part 1)"
subtitle: "The problems you can face at the beginning of your career"
date: "2021-03-04 19:03:20 +0100"
tags: ["security", "networking", "basics"]
---

As a beginner softwarer developer you probably don't care much about
certificates, private keys and other things related to security of your apps.
You just stick to good old HTTP, make sure you didn't forget to paste all of
these weird `--insecure --notls --ignore-certificate-errors 
--sure-i-want-free-bitcoins` flags, skip all warnings...

Your main goal is just to make things work, and in this early stage **there's
nothing wrong with that**! And... security can wait.

# So, will I ever need to deal with this stuff?

Then, as time passes, you start to feel that you know your favorite language in
and out. You develop project after project — thanks to the framework you picked
up. You know all the tools that might come handy when building your
appplication. Your applications do whatatever you want them to do. And you've 
finally made it — you've got your first junior position.

# Nothing can break the spell, right?
First days of work. All of a sudden, the issue that was completely out of your 
interest is back with a vengeance. It's **authentication**.

Hell breaks loose. Your brain desperately tries to parse all these error
messages, documentation pages and StackOverflow threads. All of these have
something in common — they are flooded with some mysterious acronyms like **SSL,
TLS, CA, X.509, CSR, RSA**...

*I bet you had to dive into some really advanced stuff. These problems won't
occur too often, right?*

**Unfortunately, that's not the case**. In fact, if you're unaware, you may
have to face these problems really soon.  

# Any examples?

Let's assume that...

**...communication between your apps must be *encrypted*, so you've been told to
generate some *certificates*.**

*That's no problem! I've generated hundreds of them with my Udemy account!*

**...your teammate apparently has a problem with that huge *"Your connection is
not private"* warning being your new landing page.**

*Man, how did you not know that!? Look, you just click on Advanced, then at
the bottom there's...*

**...your team has an artifact repository. Of course, it uses a *self-signed*
certificate.**

`What?`  
`Your FAVORITE-PACKAGE-MANAGER is evolving!`  
`Congratulations! Your FAVORITE-PACKAGE-MANAGER evolved into
FANCY-ERROR-PRINTER!`

*Okay, now I'm in trouble...*

# So what this whole "authentication" is about?

Without at least basic level of understanding of commonly used authentication
mechanisms, one can get really confused when moving to a professional working
environment. One way to get away from trouble is just to look for a solution
shared by someone else, copy & paste it and move on.  

Hovewer, I'd like to encourage you to take more holistic approach here.
**Authentication is ubiquitous and plays a very important role in digital
world.** It is essential for safety of network communication and provides a
fundamental source of trust on the Internet. That being said, we will take a 
closer look at every building block of authentication mechanism to understand 
it better.

In this series of articles I will explain the basics of authentication and make
all the related terminology a little clearer. You can also expect me to show 
you examples of common situations, when such knowledge may come handy.

Stay tuned!
