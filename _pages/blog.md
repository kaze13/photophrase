---
layout: page
title: Blog
include_in_header: true
---

# Blog

Here you will find all the blog posts.

{% for page in site.pages %}
  {% if page.dir == '/_pages/' %}
    <h2><a href="{{ page.url | relative_url }}">{{ page.title }}</a></h2>
    {{ page.content | markdownify }}
  {% endif %}
{% endfor %}