---
layout: default
title: Home
permalink: /
date: 2016-09-19
---

{% include bio.md %}

{% include general-info.md %}

<div class="list">
<ul class="news">
  {% for post in site.data.news.news %}
  <li class="news">
    <span class="news-date">{{ post.date | date: "%Y-%m-%d" }}</span>
    <span class="news-content">{{ post.content }}</span>
  </li>
  {% endfor %}
</ul>
</div>