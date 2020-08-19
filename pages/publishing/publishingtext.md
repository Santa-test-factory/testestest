---
layout: page
title: Publishing text
categories: publishing
group: publishing
sort_order: 4
---

This is a filler for publishing content.

<div id="archives">
{% for category in site.categories %}
 {% capture category_name %}{{ category | first }}{% endcapture %}
  {% if category_name == "publishing" %}
  <div class="archive-group">
    
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>

    <h3 class="category-head">{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories[category_name] %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
  {% endif %}
  
{% endfor %}
</div>
