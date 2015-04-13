---
title: "Better Fonts in Java Applications on Ubuntu Based Systems "
layout: post
tags: java linux ubuntu font infinality
---


On Ubuntu based systems, fonts of Java applications looks ugly. Default font-rendering in openjdk sucks anyway. Especially for developers, using popular IDEs with these fonts kills productivity. Here is the fix:

First, install Infinality:

```
sudo add-apt-repository ppa:no1wantdthisname/ppa
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install fontconfig-infinality
```

Then, install(actually upgrade) OpenJDK7 with font fixes.

```
sudo add-apt-repository ppa:no1wantdthisname/openjdk-fontfix
sudo apt-get update
sudo apt-get upgrade
```
