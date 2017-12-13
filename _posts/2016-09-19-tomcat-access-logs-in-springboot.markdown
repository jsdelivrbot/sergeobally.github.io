---
layout: post
title:  "Tomcat access logs in SpringBoot"
date:   2016-09-19 20:03:11
categories: springboot
redirect_from: "/springboot/2016/09/19/tomcat-access-logs-in-springboot.html"
comments: true
---

If you're running your SpringBoot app using Embedded Tomcat it may be useful to generate the access logs.

To do this add the following config to your application.properties file:

{% highlight java %}
server.tomcat.accesslog.enabled=true
server.tomcat.basedir=tomcat
{% endhighlight %}

Alternatively, the property values can be passed as command line options.

The result will be a new directory called tomcat at the same level as the JAR under which your logs will be created.

SpringBoot version: `1.4.0-RELEASE`
