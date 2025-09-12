---
layout: home
title: Blog
---

## My Blog Posts

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.date | date: site.date_format }}</p>
    {% if post.excerpt %}
      {{ post.excerpt }}
    {% endif %}
  </article>
{% endfor %}
