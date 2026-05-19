---
layout: default
title: 首页
---

<h1>欢迎来到我的博客</h1>

<p>这是我的个人博客，记录学习与生活。</p>

<h2>最新文章</h2>

{% for post in site.posts %}
  <article class="post-preview">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.date | date: "%Y年%m月%d日" }}</p>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}
