---
layout: archive
title: Prácticas de Procesadores de Lenguajes
permalink: /practicas/
---

<ul>
{% for practica in site.data.practicas %}
    <li>
      <h3>{{ practica.name }}</h3>
      <p> Tema: {{ practica.topic }}</p>
    </li>
{% endfor %}
</ul>