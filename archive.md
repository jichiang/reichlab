---
layout: default
title: Blog
---

## Blog Posts

{% for post in site.posts %}
  * [ {{ post.title }} ]({{ post.url }}) &raquo; {{ post.date | date_to_string }}  
{% endfor %}