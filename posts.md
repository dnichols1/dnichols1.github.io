---
layout: single
title: All Posts
author_profile: true
permalink: /posts/
---

{% for post in site.posts %}  
  {% include archive-single.html %}
{% endfor %}

