---
layout: home
title: Welcome to CBYun-Blog
---

Hi! 👋 This is my personal blog powered by GitHub Pages and ChatGPT.

Below are my latest posts:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
