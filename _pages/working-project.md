---
layout: archive
title: "Working Project"
permalink: /working-project/
author_profile: true
---

{% include base_path %}

*Papers currently in progress, under review, or in preparation.*

{% for post in site.publications reversed %}
  {% if post.category != "in_progress" %}
    {% continue %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}
