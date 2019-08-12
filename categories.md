---
layout: single
title: Posts by Category
author_profile: true
permalink: /categories/
---

{% for category in site.categories %}
  <h3 class="archive__subtitle"><a name="{{ category | first }}">{{ category | first }}</a></h3>
  {% for post in category.last %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}

