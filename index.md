---
title: .
---
# Welcome to the c4u-bpm-poc-maco docu!

<p>These are the categories for all blog posts:</p>
<ul>
{% for category in site.categories %}
<li><a href="{{ site.url }}/testestest/category/{{ category | first | url_encode }}/index.html">{{ category | first }}</a></li>
{% endfor %}
</ul>
<p>They link to the corresponding index pages!</p>

[About BPM](about.md)
