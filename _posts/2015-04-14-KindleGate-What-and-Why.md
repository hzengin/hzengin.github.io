---
title: "KindleGate, What and Why?"
layout: post
tags: kindle amazon epub mobi
---

Recently, I tought that trusting Amazon about handling and storing my ebooks is a little freaky, clearly Amazon is a company which has responsibilties to law and aims to earn money, acctually even if I don't have any illegal stuff like pirate ebooks, manuals to make a nuke etc. my ebooks gives an inside and briliant opinion about my personality which I don't want at all. This is why I created the tiny application called [KindleGate](http://github.com/hzengin/KindleGate).

## What is KindleGate?

KindleGate is a tiny python+flask application that lists, searchs my epubs and converts them to downloadable mobis when I requested for. 
Providing web interface with flask that I can access directly from my Kindle and ebook convertion with calibre's ebook-convert tool, KindleGate became a inseparable part of life.

### Usage:
1. Clone It
2. Change epubs directory at `Utilities.py`
3. Change crediantals directory at `Authentication.py`
4. Run it `python3 KindleGate.py`
5. Connect it via browser from Kindle, search or see full list and click a epub to download and start reading!

Here is how homepage looks like just after login:
![Screenshot]({{ site.url }}/assets/ss.png)
