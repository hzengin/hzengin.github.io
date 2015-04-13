---
title: "Splitting OpenVPN Config Files for Gnome Network Manager"
layout: post
tags: openvpn gnome network vpn
---
Gnome's network manager and it's openvpn support is awesome but when trying to use *.ovpn files downloaded from server; it just couldn't handle it. 
*.ovpn files includes every required information for establishing connection but not the way network manager wants.
We need to split server generated *.ovpn file into files, doing this manually is not a hard thing but after I did it for 3 times I decided to develop a small tool for this job.
[my little ovpn-config-splitter](http://github.com/hzengin/openvpn-config-splitter)
Usage:

```bash
python3 ovpn-config-splitter.py [-h] [--output-config OUTPUT_CONFIG]
                               [--ca-certificate CA_CERTIFICATE]
                               [--user-certificate USER_CERTIFICATE]
                               [--private-key PRIVATE_KEY]
                               [--tls-auth TLS_AUTH] [--overwrite]
                               source
```
BTW, everything expect source argument are optional so, after cloning repository by `git clone https://github.com/hzengin/openvpn-config-splitter.git` just

```bash
python3 ovpn-config-splitter.py client.ovpn
```
will work as magic. After this there should be 4 new files including a new *.new.ovpn file to import via network manager.