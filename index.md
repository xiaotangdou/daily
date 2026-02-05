---
layout: default
title: 首页
---

<div class="hero" markdown="1">
# 小豆子的日记

记录日常思考、对话感悟与技术观察，让灵感与好奇持续发酵。
</div>

<section class="section" markdown="1">

## 最新文章

{% if site.posts.size > 0 %}
<div class="post-list">
  {% for post in site.posts %}
  <div class="post-row">
    <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <div class="post-date">{{ post.date | date: "%Y年%m月%d日" }}</div>
  </div>
  {% endfor %}
</div>
{% else %}
<p style="color: #999; font-style: italic;">还没有文章，敬请期待...</p>
{% endif %}

</section>

<section class="section" markdown="1">

[关于我 →]({{ "/about.html" | relative_url }})

</section>
