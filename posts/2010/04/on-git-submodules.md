<!--
id: 553870821
link: http://tumblr.atmos.org/post/553870821/on-git-submodules
slug: on-git-submodules
date: Tue Apr 27 2010 11:09:00 GMT-0700 (PDT)
publish: 2010-04-027
tags: 
title: on git submodules
-->


on git submodules
=================

Christopher Stolt: I have a few questions about using git submodules if
you have a couple of minutes to discuss Corey Donohoe: the answer is,
don't Christopher Stolt: don't use them? Corey Donohoe: some people like
them Corey Donohoe: i don't really, they work fine tho Corey Donohoe:
it's basically a subdir in your project that points to another git repo
Christopher Stolt: I think for what these guys are doing they'd make
sense...at least my understanding of them Christopher Stolt: yeah
Christopher Stolt: these guys have 4 apps that all share the same code
in their models dir Corey Donohoe: usually submodules are cases where
packaging is either a) really fucking slow to dev or b) complete shit
Corey Donohoe: if they wanna share models they should really revision
gems Christopher Stolt: interesting Corey Donohoe: the idea being that
all of their models live in a gem and you ensure that all four apps are
on the same version w/ some history Corey Donohoe: versus updating
submodules in each app, they simply upgrade Corey Donohoe: it's how we
do it here fwiw Christopher Stolt: makes total sense and if they were
bundling it'd be even easier to make sure they were requiring the proper
gem Corey Donohoe: yup Christopher Stolt: and it'd allow them to work
out of branches without issues too Corey Donohoe: and it requires some
coordination between the four apps the pause the developer does to say
"how will this impact all four apps" is usually a good reflection point
Christopher Stolt: thanks man Corey Donohoe: np

