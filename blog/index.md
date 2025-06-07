---
layout: blog
title: Blog
---
# Mein Blog

<div class="blog-list">
{% for post in site.posts %}
  <article class="blog-list-item">
    {% if post.image %}
    <img src="{{ site.baseurl }}{{ post.image }}" alt="">
    {% endif %}
    <div>
      <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title | default: post.slug }}</a></h2>
      <small>{{ post.date }}</small>
      <p>{{ post.excerpt | strip_html | truncate: 140 }}</p>
    </div>
  </article>
{% endfor %}
</div>