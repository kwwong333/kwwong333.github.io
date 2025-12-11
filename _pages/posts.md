---
layout: archive
permalink: /posts/
title: "Posts"
author_profile: true
---

{% include base_path %}

<h2>Browse by tag</h2>
<ul>
  {% for tag in site.tags %}
    <li>
      <a href="{{ base_path }}/tag/{{ tag[0] | slugify }}/">
        {{ tag[0] }} ({{ tag[1].size }})
      </a>
    </li>
  {% endfor %}
</ul>

<hr>

{% for post in site.posts reversed %}
  {% include archive-single.html %}
{% endfor %}
