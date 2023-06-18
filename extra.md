---
layout: default
title: About
permalink: /extra
---
# ЭКСТРА

<ul class="post-list archive-ul">
  {% for post in site.categories.extra %}
    <li class="archive-li">
      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>
