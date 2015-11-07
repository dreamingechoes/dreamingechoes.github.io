---
layout: tip
title: "Install old versions therubyracer gem on Mac OS X."
date: 2015-10-31 15:30:00
categories: gem ruby rails
tags: gem ruby rails development web therubyracer
comments: true
excerpt: "Install old version of therubyracer gem on Mac OS X without pain."
post_summary: "Install old version of therubyracer gem on Mac OS X without pain."
image:
  feature: header-image.png
url: http://dreamingechoes.github.io/tips/install-old-versions-therubyracer-gem-on-mac-os-x/
---

I had a problem when I tried to install version 0.10.2 of therubyracer gem on Mac OS X Yosemite, so I searched and I tried different solutions, and the one it works for me was this:

```sh
brew tap homebrew/dupes
brew install apple-gcc42

export CC=/usr/local/Cellar/apple-gcc42/4.2.1-5666.3/bin/gcc-4.2
export CXX=/usr/local/Cellar/apple-gcc42/4.2.1-5666.3/bin/g++-4.2
export CPP=/usr/local/Cellar/apple-gcc42/4.2.1-5666.3/bin/cpp-4.2

brew uninstall v8

gem uninstall libv8

gem install therubyracer -v '0.10.2'
```

## Any place where I can pick the code of this tip?

Yeah! Here you have the [Github gist](https://gist.github.com/dreamingechoes/9b76b7eaf86ff1961804) for this tip :)
