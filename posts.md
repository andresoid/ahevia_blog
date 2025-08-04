---
layout: default
title: Posts
permalink: /posts/
---

# Todos los Posts

<div class="post-list">
{% for post in site.posts %}
  <div class="post-list-item">
    <h2 class="post-list-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>
    <p class="post-list-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">
        {{ post.date | date: "%d de %B de %Y" }}
      </time>
      {% if post.author %} • {{ post.author }}{% endif %}
    </p>
    {% if post.excerpt %}
      <div class="post-list-excerpt">
        {{ post.excerpt }}
      </div>
    {% endif %}
  </div>
{% endfor %}
</div>

{% if site.posts.size == 0 %}
<p>Aún no hay posts publicados. ¡Vuelve pronto para ver nuevo contenido!</p>
{% endif %}
