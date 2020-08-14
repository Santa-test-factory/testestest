---
layout: page
title: Publishing
categories: publishing
---

This is a filler for publishing content.

{% for post in site.categories.publishing %}
 <li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
