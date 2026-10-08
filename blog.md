---
title: Blog
layout: default
---

{% if site.posts.size == 0 %}
<p>Aucun article pour le moment. Restez à l'affût !</p>
{% else %}
{% for post in site.posts %}
<div class="post-card">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-date">Publié le {{ post.date   date_to_string }}</p>
    {% if post.excerpt %}{{ post.excerpt | strip_html | truncatewords: 25 }}{% endif %}
</div>
{% endfor %}
{% endif %}
