<!--
id: 28313931
link: http://tumblr.atmos.org/post/28313931/irssi-growl-on-leopard-with-macports
slug: irssi-growl-on-leopard-with-macports
date: Sat Mar 08 2008 11:42:00 GMT-0800 (PST)
publish: 2008-03-08
tags: 
title: irssi + growl on leopard with macports
-->


irssi + growl on leopard with macports
======================================

-   Install Growl
-   % sudo port install irssi +perl
-   Grab the Growl SDK from http://growl.info/downloads\_developers.php
-   Copy the Bindings folder from the DMG to your homedir
-   % sudo port install -f p5-mac-osa-simple p5-mac-glue
-   % cd \~/Bindings/perl/Mac-Growl
-   % perl Makefile.PL; sudo make; sudo make install
-   Grab the OLD growl release, 0.7.6. [Growl
    .7.6](http://growl.info/files/Growl-0.7.6.dmg)
-   % mkdir -p \~/.irssi/scripts/autorun
-   % cp /Volumes/Growl/Scripts/irssi/growl.pl \~/.irssi/scripts/autorun
-   % irssi
-   shift+fn+up scrolls up in Terminal.app.  You can also grab the
    IRSSI.terminal file I uploaded to pastie that makes pg-up work by
    default([http://pastie.caboo.se/163371](http://pastie.caboo.se/163371)).


