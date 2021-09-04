---
layout: default
title: Blog
description: "List of blog posts"
nav_exclude: true
permalink: /blog/
---

{% for post in site.posts %}
  <article>
    <p class="text-small dateinmylist nospaces">{{ post.date | date: "%B %-d, %Y" }}</p>
    <a class="titleinmylist" href="{{ post.url }}">{{ post.title }}</a>
    {{ post.excerpt }}
    <hr>
  </article>
{% endfor %}