---
layout: default-blog
title: Blog
---

<div id="sub-header">  
{% for post in site.posts %}
<!-- #sub-header -->

  <div class="container">
    <h1 class="entry-title">
      <a href="{{ post.url | prepend: site.baseurl | prepend: site.url }}">{{ post.title }}</a>
    </h1>
      <p>{{ post.date | date: "%d/%m/%y" }}</p>
  </div>

<!-- #sub-header end -->
{% endfor %}
</div>