---
layout: post
title:  "Using Nginx in node app development"
author: Harry Gill
tags:
  - nginx
  - JavaScript
  - nodejs
  - cookie-session
date:   2016-12-09 22:01:43
categories: ["nginx", "nodejs"]
---
  I have been worknig on a personal project using nodejs for both frontend and backend.
It was going fine until I started using [cookie-session] (https://github.com/expressjs/cookie-session).
When you login on the server and it authenticates and sends a cookie back to the browser,
The issue I faced was both by devservers and frontend and backend are running on diffrent ports
so the client doesn't stored and send the cookie back to server at all.

for example my backend and frontend dev servers were running on port 3000 and 8080 respectively.

---

One way to solve this problem is using a [Nginx](https://www.nginx.com/) server as a as reserve proxy.

{% highlight bash %}
$ sudo apt-get install nginx
{% endhighlight %}

## TBC.... soon ##
