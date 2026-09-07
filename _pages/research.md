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

{% include base_path %}

<h2 style="font-size: 1.8em; margin-top: 0.5em; margin-bottom: 0.8em;">Working Papers</h2>

{% assign sorted_research = site.research | sort: "date" | reverse %}
{% for post in sorted_research %}
  {% if post.category == "working" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2 style="font-size: 1.8em; margin-top: 1.2em; margin-bottom: 0.8em;">Work in Progress</h2>

{% assign sorted_research = site.research | sort: "date" | reverse %}
{% for post in sorted_research %}
  {% if post.category == "ongoing" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
