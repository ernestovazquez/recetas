---
layout: default
title: Platos de Fondo
permalink: /categories/platos-de-fondo/
---

<main class="page-content" aria-label="Content">
  <section class="recent_box">
    <div class="post_wrapper">
      <h2 class="recent_title">Platos de Fondo</h2>

      <div class="recent_list">
        {% for post in site.tags['platos-de-fondo'] %}
          <a href="{{ post.url | prepend: site.baseurl }}" class="recent_item">
            <div class="post-thumbnail" style="background-image: url('{{ "/assets/img/" | prepend: site.baseurl | append: post.img }}');">
              <span class="post-title">{{ post.title }}</span>
            </div>
          </a>
        {% endfor %}
      </div>

      <div class="back_to_home">
        <a href="{{ site.baseurl }}/" class="back-link"><i class="fa fa-long-arrow-left" aria-hidden="true"></i>   Back</a>
      </div>
    </div>
  </section>
</main>

{% include footer.html %}

