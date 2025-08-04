---
title: Bienvenido
layout: default
---

# 👋 ¡Hola!

Bienvenido a mi blog personal donde escribo sobre cosas que me interesan de TI: programación, tecnología, arquitectura, clouds, y por supuesto inteligencia artificial.

## Posts Recientes

<div class="post-list">
{% for post in site.posts limit:5 %}
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
{% else %}
<p><a href="{{ '/posts' | relative_url }}">Ver todos los posts →</a></p>
{% endif %}

## Sobre este blog

Aquí comparto mis experiencias, aprendizajes y reflexiones sobre:

- **Programación** y desarrollo de software
- **Arquitectura** de sistemas y aplicaciones
- **Cloud Computing** y DevOps
- **Inteligencia Artificial** y Machine Learning
- **Tecnología** en general

¿Quieres saber más? Visita la página [Acerca de]({{ '/about' | relative_url }}) para conocer más detalles.
