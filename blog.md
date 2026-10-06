---
title: Blog
---

# Blog ReLiance

Nombre d'articles détectés : **{{ site.posts.size }}**

{% for post in site.posts %}
- {{ post.title }} — {{ post.date   date: "%d/%m/%Y" }}
{% endfor %}
