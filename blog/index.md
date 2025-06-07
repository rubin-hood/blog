---
layout: home
title: Blog
---
# Mein Blog
{% for post in site.posts %}
  <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
{% endfor %}
