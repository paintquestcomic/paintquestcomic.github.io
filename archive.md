---
layout: default
title: Архив
permalink: /archive
---
# Архив

<ul class="post-list archive-ul">
  {% for post in site.categories.page %}
    <li class="archive-li">
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>
