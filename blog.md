---
layout: page
title: Blog
permalink: /blog/
---

# Blog Posts
{% for post in site.posts %}
- **{{ post.date | date: "%Y-%m-%d" }}** &nbsp; [{{ post.title }}]({{ post.url }})
{% endfor %}
