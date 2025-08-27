---
layout: default
title: Home
---

<section class="card">
  <h2>観測エロティクス小品集へようこそ</h2>
  <p>ここは <strong>観測・干渉・波動関数</strong> を官能的な暗喩として読み解く実験場。数式でゾクゾクし、物理でとろける人のための場所です。</p>
  <div class="warning">
    <strong>注記：</strong> 本サイトは科学的な暗喩表現を含みます。露骨な性描写は避け、<em>知覚としての官能</em>を追究します。
  </div>
</section>

<h3>最新の短編</h3>
<div class="post-grid">
  {% for post in site.posts limit:6 %}
    <div class="post-card">
      {% if post.image %}
        <a href="{{ post.url | relative_url }}"><img src="{{ post.image | relative_url }}" alt="{{ post.title }}"></a>
      {% endif %}
      <h4><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h4>
      <div class="small">{{ post.date | date: "%Y-%m-%d" }}</div>
      <p>{{ post.excerpt | strip_html | truncate: 100 }}</p>
    </div>
  {% endfor %}
</div>

<h3>Stories コレクション</h3>
<ul>
  {% for item in site.stories %}
  <li><a href="{{ item.url | relative_url }}">{{ item.title }}</a></li>
  {% endfor %}
</ul>
