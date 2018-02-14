---
title: My experience with trying to deploy different packages quickly
date: 2018-02-13 16:55:00 Z
categories:
- coding
tags:
- git
- coding
- github
- workshop
- tate
---

I was running a identifier workshop at the tate modern and I was chosen the run a networking workshop. The microbits have radio functions but we needed the make sure everyone had a special different identifier variable so I decided to create the code for all ten pi-tops. Ten minutes later I had all the hex files and I needed to be able to deploy them on all machines within ten minutes in a day. I decided to do this via `git`. It probably was not the best idea. I ended having to create individual branches for each variable and it ended up taking over two hours. When I was done I made a simple bash script that I could `curl` down from github and add a variable to the end for the microbit numbers.
~~~
#! /bin/bash/

git clone -b $1 https://github.com/evanwaltersdev/yccpreload.git
~~~
It ended up being a unique experience for me to learn these git skills because they will certainly be required in the future. 