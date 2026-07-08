---
layout: default
title: Главная
---

# Корпоративная тревога и AI

{% for post in site.posts %}
<article class="post-card">
  {% if post.image %}
  <a href="{{ post.url | relative_url }}"><img src="{{ post.image | relative_url }}" alt="{{ post.title }}"></a>
  {% endif %}
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.description }}</p>
  <a class="read-more" href="{{ post.url | relative_url }}">Читать →</a>
</article>
{% endfor %}
