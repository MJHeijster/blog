---
title: "Cordova/PhoneGap NO TRANSPORT/NetworkError with Ajax in Windows Phone."
date: "2013-05-08"
categories: 
  - "blogs"
tags: 
  - "ajax"
  - "jquery-mobile"
  - "windows-phone"
coverImage: "jqm1.png"
---

_When developing for multiple platforms, a framework might be nice. One of those frameworks is Cordova a.k.a. PhoneGap. When using jQuery Mobile, I stumbled upon the problem that I couldn't do an ajax request to an API in Windows Phone. The same code did work for Android. After searching for a while, I found out that this problem is known and that it will not be fixed. There is, however, a workaround._

# What's happening

In Windows Phone cross-domain ajax calls are blocked.

# How to solve

The bug was reported back in 2011 for jQuery. They decided not to fix it for jQuery Mobile. Instead they suggested to use **$.support.cors = true;**.

This does solve the problem for the calls.

# Example code

\[js\]$.support.cors = true;

$.ajax("http://localhost:8081/api.html", { async: false, contentType: "text/xml", data: body, type: "POST", success: function (data, textStatus, jqXHR) { //Handle the api call }, error: function (jqXHR, textStatus, errorThrown) { //Handle the error } });\[/js\]
