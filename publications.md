---
layout: default
title: Publications
---

<h1>Publications</h1>
<br />

<hr /><br />

{% for post in site.posts %}
  <div class="publication">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
    <img src="path/to/your/image.jpg" alt="Image description" class="right-image" />
    <hr />
  </div>
{% endfor %}
