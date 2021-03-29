---
layout: single
title: Authors
permalink: /authors/
excerpt: "Authors contributing in this page."
---

<ul>
  {% for author in site.authors %}  
    <li>
      <h2>{{ author.name }} - {{ author.position }}</h2>
      <p>{{ author.content | markdownify }}</p>
    </li>
  {% endfor %}
</ul>
