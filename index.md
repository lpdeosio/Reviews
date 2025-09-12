---
layout: home  # Use Minima's home layout for post previews if desired
title: Home
---

# Welcome to Lloyd De Osio's Blog

![Banner](banner.jpg)  <!-- If banner is an asset; upload if needed -->

Experienced remote professional with a strong foundation in US healthcare, administrative assistance, finance operations.

## Navigation
- [Blog](/blog/) – Read my latest posts
- [Email Me](mailto:lpdeosio@gmail.com)

{% if site.posts.size > 0 %}
## Recent Posts
{% for post in site.posts limit:3 %}
  <article>
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p>{{ post.date | date: site.date_format }}</p>
    {{ post.excerpt }}
  </article>
{% endfor %}
{% endif %}
