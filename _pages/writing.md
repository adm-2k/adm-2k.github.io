---
title: "Writing"
permalink: /writing/
redirect_from:
  - /posts/
kicker: "Notes & essays"
lede: >-
  Occasional notes on civic tech, teaching, open source, and language.
  Plain Markdown, no algorithm — subscribe by
  <a href="/feed.xml">RSS</a> if you'd like.
---

<ul class="post-list">
  {% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
  </li>
  {% endfor %}
</ul>
