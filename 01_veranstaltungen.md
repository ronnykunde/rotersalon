---
bg: "DSC_3162-copy.jpg"
layout: page
permalink: /veranstaltungen/
title: "Veranstaltungen"
crawlertitle: "Veranstaltungen"
summary: ""
active: veranstaltungen
---

{% for post in site.categories.Veranstaltungen %}
  <article class="veranstaltungen-page">
  	<img src="../assets/images/thumbnails/{{ post.bg }}" />
  	<a href="{{ post.url | relative_url }}">
	  	 <p class="post-meta">{{ post.date | date: "%d.%m.%Y"}}</p>
	    <h2>{{ post.title }}</h2>
	    <h4>{{ post.subtitle }}</h4>
    </a>
  </article>
{% endfor %}