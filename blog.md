---
title: Blog
---

# Blog ReLiance

Nombre d'articles détectés : {{ site.posts.size }}

{% for post in site.posts %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<p>Publié le {{ post.date   date: "%d/%m/%Y" "}}</p>
{% endfor %}
