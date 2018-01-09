---
layout: default
title: Start Here
navexclude: true
---

{% for item in site.learn %}
{% unless item.navexclude == true %}
  <h2>{{ item.title }}</h2>
  <p>{{ item.description }}</p>
  <p><a href="{{ item.url }}">{{ item.title }}</a></p>
{% endunless %}
{% endfor %}