---
layout: default
title: Categorías
permalink: /categories/
---

<section class="categories-list">
  <div class="container">
    <h2>Todas las Categorías</h2>
    <ul>
      {% for category in site.categories %}
        <li><a href="/categories/{{ category | first }}/">{{ category | first }}</a></li>
      {% endfor %}
    </ul>
  </div>
</section>

