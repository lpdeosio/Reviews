---
layout: default
title: Blog
---

<nav>
  <a href="/">← Home</a>
</nav>

<h1>My Blog Posts</h1>

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
    <article>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>Posted on {{ post.date | date: site.date_format }}</p>
      {% if post.excerpt %}
        <div class="excerpt">{{ post.excerpt | strip_html }}</div>
      {% endif %}
      <a href="{{ post.url }}">Read full post →</a>
    </article>
    <hr>
  {% endfor %}
{% else %}
  <p>No posts yet—check back soon!</p>
{% endif %}
