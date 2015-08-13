---
layout: default
title: Blog
---

## Blog Posts

{% for post in site.posts %}
  * [ {{ post.title }} ]({{ site.baseurl }}{{ post.url }}) &raquo; {{ post.date | date_to_string }}  
{% endfor %}