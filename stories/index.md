---
layout: default
title: Stories
permalink: /stories/
---

<p>連作やテーマ別の小品はここにまとめます。</p>
<ul>
{% for item in site.stories %}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a></li>
{% endfor %}
</ul>