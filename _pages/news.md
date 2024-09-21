---
layout: archive
permalink: /news/
title: "News"
author_profile: true
redirect_from:
  - /wordpress/blog-posts/
---

{% include base_path %}

{% for post in site.news reversed %}
  {% include archive-single.html %}
{% endfor %}
