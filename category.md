---
layout: default
title: Categories
---
<h1>Categories</h1>

{% for category in site.categories %}
  <h4>{{ category[0] | upcase}}</h4>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
