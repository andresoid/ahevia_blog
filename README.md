# Blog Personal de Andrés Hevia

[![Build and Deploy Jekyll](https://github.com/andresoid/ahevia_blog/actions/workflows/jekyll-gh-pages.yml/badge.svg)](https://github.com/andresoid/ahevia_blog/actions/workflows/jekyll-gh-pages.yml)

Mi blog personal donde escribo sobre TI, programación, tecnología, arquitectura, clouds e inteligencia artificial.

## 🌐 Sitio Web

El blog está disponible en: [https://andresoid.github.io/ahevia_blog/](https://andresoid.github.io/ahevia_blog/)

## 🛠️ Tecnologías

- **Jekyll 4.3**: Generador de sitios estáticos
- **GitHub Pages**: Hosting gratuito
- **GitHub Actions**: CI/CD automatizado
- **Markdown**: Para escribir contenido
- **Sass**: Para estilos CSS
- **Rouge**: Syntax highlighting

## 📁 Estructura del Proyecto

```
├── _config.yml          # Configuración de Jekyll
├── _layouts/            # Plantillas HTML
├── _includes/           # Componentes reutilizables
├── _sass/              # Archivos SCSS
├── _posts/             # Posts del blog
├── assets/             # CSS, JS, imágenes
├── .github/workflows/  # GitHub Actions
├── Gemfile             # Dependencias Ruby
└── index.md            # Página principal
```

## 🚀 Desarrollo Local

### Prerrequisitos

- Ruby 3.1 o superior
- Bundler

### Instalación

1. Clona el repositorio:
```bash
git clone https://github.com/andresoid/ahevia_blog.git
cd ahevia_blog
```

2. Instala las dependencias:
```bash
bundle install
```

3. Ejecuta el servidor local:
```bash
bundle exec jekyll serve
```

4. Abre tu navegador en `http://localhost:4000`

### Comandos Útiles

```bash
# Servir el sitio localmente
bundle exec jekyll serve

# Servir con drafts
bundle exec jekyll serve --drafts

# Construir el sitio
bundle exec jekyll build

# Limpiar archivos generados
bundle exec jekyll clean
```

## ✍️ Escribir un Post

1. Crea un nuevo archivo en `_posts/` con el formato: `YYYY-MM-DD-titulo.md`

2. Agrega el front matter:
```yaml
---
layout: post
title: "Título del Post"
date: YYYY-MM-DD HH:MM:SS -0300
categories: [categoria1, categoria2]
tags: [tag1, tag2, tag3]
author: Andrés Hevia
excerpt: "Descripción breve del post"
---
```

3. Escribe el contenido en Markdown

4. Usa `<!--more-->` para separar el excerpt del contenido completo

## 📝 Configuración de GitHub Pages

El sitio se despliega automáticamente usando GitHub Actions cuando se hace push a la rama `main`.

### Configuración en GitHub:

1. Ve a Settings → Pages
2. Source: GitHub Actions
3. El workflow se ejecutará automáticamente

## 🎨 Personalización

### Colores y Estilos

Edita los archivos en `_sass/` para personalizar:
- `_base.scss`: Estilos base
- `_layout.scss`: Layout y componentes
- `_syntax-highlighting.scss`: Colores del código

### Configuración del Sitio

Edita `_config.yml` para cambiar:
- Título y descripción
- URL del sitio
- Configuración de plugins
- Configuración de navegación

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si encuentras un error o tienes una sugerencia:

1. Abre un Issue
2. Fork el proyecto
3. Crea una rama para tu feature
4. Envía un Pull Request

---

⭐ Si te gusta este proyecto, ¡dale una estrella en GitHub!
