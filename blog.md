---
layout: default
title: Blog
---

# Blog

{% if site.posts.size > 0 %}
<ul class="posts">
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
  </li>
{% endfor %}
</ul>
{% else %}
<p class="empty">Coming soon.</p>
{% endif %}
