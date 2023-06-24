---
layout: default
title: Архив
permalink: /archive
---
<h1 class="section-title">Архив</h1>

<div class="archive">
  {% for post in site.categories.page reversed %}
  {% if post.permalink == "/001" %}
  <h2>Пролог: Гладиоратор</h2>
  {% endif "%}

  {% if post.permalink == "/035" %}
  <h2>Глава 1: Немые Сцены</h2>
  {% endif "%}

  {% if post.permalink == "/088" %}
  <h2>Глава 2: Партнёрство Сомнительной Добросовестности</h2>
  {% endif "%}

  {% if post.permalink == "/154" %}
  <h2>Глава 3: Великое Ремесло</h2>
  {% endif "%}

  {% if post.permalink == "/177" %}
  <h2>Глава 4: ЭСХТ</h2>
  {% endif "%}
        <p>
          <strong>{{ post.date | date: "%d.%m.%Y" }}</strong> - <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </p>
  {% endfor %}
</div>
