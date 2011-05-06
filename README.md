The facts
=========

MicroJS is the tiniest Javascript micro-library, with **Only 10 bytes** !

No bloatware, only the essential. MicroJS is minimalist, you have to add your own tools and use them the way you like or need.
MicroJS is not a framework, it should be more considered as a framework builder ! Build your own favorite tools with this incredibly blazing fast factory !!

Usage
=====

Include
-------

    <script src="/path/to/micro.js"></script>

You can put it in your `<head>`, `<body>` or whatever, it's so small it won't matter.

CDN
---

MicroJS is not available in CDNs, but who cares, it's so small :D

Configure
---------

Once MicroJS is loaded, you're now free to configure it the way you like.

Include your additional libraries, and merge them into MicroJS this way to declare plugins :

    µ.tool = tool

Any valid JS expression can be a plugin, full freedom !!!

Use your tools
--------------

Once you've added your tools, feel free to use them, in a standard way, thanks to MicroJS :D All your plugins can now be called in a homogenous, easy to remember, way :

    µ.tool(…)

Sample
======

A plugin that allow to hide or show elements :

    // hide/show plugin
    µ.toggle = function(e){e.style.display=e.style.display=='none'?'':'none'}

A simple way to use your own DOM selector :

    µ.$ = qwery

You can even combine them ! Full freedom I said !!

    µ.toggle(µ.$('#hide-me'))
