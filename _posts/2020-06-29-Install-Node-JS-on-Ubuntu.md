---
layout: post
title: Install Node.js on Ubuntu
date:   2020-06-29 14:38:00
categories: Node.js
---

## Install Node.js on Ubuntu

The simplest way to install Node.js on Ubuntu:

```
sudo apt install curl
curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
sudo apt-get install -y nodejs
sudo apt-get install gcc g++ make
node --version
npm --version
```

![node.js](/assets/nodejs.png)