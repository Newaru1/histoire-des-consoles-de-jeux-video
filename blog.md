---
layout: default
title: Histoire des consoles
permalink: /articles/
---
<h1>
  Histoire des consoles
</h1>

{% assign sorted_posts = site.posts | sort: 'date' | reverse %}

{% for post in site.posts %}
<article class="blog-item">
  <h2>
    <a href="{{post.url | relative_url}}"> {{ post.title }} </a>
  </h2>
  <a href="{{post.url | relative_url}}"> Lire l'article ➞ </a>
</article>
<hr />
{% endfor %}
