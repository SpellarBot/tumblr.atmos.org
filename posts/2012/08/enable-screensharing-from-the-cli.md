<!--
id: 29095938374
link: http://tumblr.atmos.org/post/29095938374/enable-screensharing-from-the-cli
slug: enable-screensharing-from-the-cli
date: Thu Aug 09 2012 19:26:11 GMT-0700 (PDT)
publish: 2012-08-09
tags: 
title: enable screensharing from the cli
-->


enable screensharing from the cli
=================================

sudo
 /System/Library/CoreServices/RemoteManagement/ARDAgent.app/Contents/Resources/kickstart
-activate -configure -access -on -clientopts -setvnclegacy -vnclegacy
yes -clientopts -setvncpw -vncpw mypasswd -restart -agent -privs -all

