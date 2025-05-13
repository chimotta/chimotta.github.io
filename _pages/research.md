---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

<style>
.page__title {
  display: none;
}
</style>

<h2 style="font-size: 1.8em; margin-top: 0.5em; margin-bottom: 0.8em;">Working Papers</h2>

{% include base_path %}

{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %}
