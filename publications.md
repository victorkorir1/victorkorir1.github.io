---
layout: default
title: Publications
---

<style>
  hr {
    margin-top: 30px;
    margin-bottom: 50px;
  }
</style>

<div>
<h1>Publications</h1>
<br />

<hr /><br />

{% for post in site.posts %}

  <div class="publication">
    <h2><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
    <p>{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
    <img src="path/to/your/image.jpg" alt="Image description" class="right-image" />
    <hr />
  </div>
{% endfor %}

</div>
