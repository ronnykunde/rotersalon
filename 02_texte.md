---
bg: "DSC_3174-copy.jpg"
layout: page
permalink: /texte/
title: "Texte"
crawlertitle: "Texte"
summary: ""
active: texte
---

{% for post in site.categories.Texte %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  </article>
{% endfor %}
