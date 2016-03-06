mp3gain
=======

This repository contains all the source code you need to build aacgain on OS X 10.11 
(El Capitan), without need to look for source code on other sites.

It combines the original mp3gain repository that elfchief copied to GitHub
with the source code to build mp4v2 from the almost-defunct Google Code and 
and the source code libfaad from the SourceForge. (Remember when SourceForge 
cool like Github is now? OK I'm old. :) 
It also includes a couple patches to mp4v2.  
See the commit history for more details on exactly what was patched and included.

Instructions for compiling aacgain are in aacgain/linux/README.linux.

(If you just want mp3gain, it can be compiled 

I was able to build this with build tools I already had installed (xcode, homebrew)
plus `brew instal libtool` to resolve an error about libtool.

PLEASE NOTE that I did not write and do not claim authorship or copyright
over this code. I am posting it as a courtesy to others who may find
it useful, and believe this to be in compliance with the Open Source licenses 
used by the original authors. 

Usage
=====

For example, to update a single file to a better volume level (BACKUP YOUR FILE BEFORE
RUNNING):

    ./aacgain -r path/to/file.m4a

I found the `-r` switch was needed to make it automatically increase the level of a single
file (by default I beleive it expects more than one file to make a change).



