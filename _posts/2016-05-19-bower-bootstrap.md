---
layout: post
title: bower-bootstrap
subtitle: "Learning to user bower to get Twitter Bootstrap files in project easily."
date: 2016-05-19
tags: [Tutorial]
author: "Shaswat Gupta"
header-img: "img/autumnsky.jpg"
---

## Bower

<a style="color:#FC645F" href="http://bower.io/">Bower</a> is a front-end dependency manager for your project. In laymans terms, it is a command-line program which you can utilize to download libraries such as <a style="color:#FC645F" href="http://getbootstrap.com/">Twitter Bootstrap</a>. The beauty of this approach is that we can generate a `bower.json` file, which any user can copy and use to download a bunch of packages easily - as opposed to going to each site, and manually copy/pasting/saving out files. 

In this step, I'll walk you through downloading Twitter bootstrap as well as generating your own `bower.json`. Before we do this, we'll create a `.bowerrc` file.

In the same directory as `manage.py`, create a `.bowerrc` file with the following content:

{% highlight bash %}
{
    "directory": "app/static/"
}
{% endhighlight %}

Anytime we run `bower`, it will output the downloaded files within the directory listed here. 

<blockquote><b>Tip:</b> There is a huge array of <a style="color:#FC645F" href="http://bower.io/docs/config/">configuration options</a> which can be used, for those curious.</blockquote>


And now in our command line, we can simply run:

{% highlight bash %}
$ bower install bootstrap
{% endhighlight %}

This will download Twitter Bootstrap into our project directory,  as specified within our `.bowerrc` file. 

Thanks for reading. 
