---
layout: page
permalink: /spotlight/
title: Spotlighting our Celebrated Women of Accomplishment
tagline: FGGC Osha Alumni Chapter
tags: [profile]
modified: 5-9-2015
comments: true
---

Check out all our spotlight articles

<div id="index">
 <article>
  {% for post in site.categories.spotlight %}
  <h2><a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: '%D' }} </p>
  <br>
  <p>{% if post.description %}{{ post.description }}{% else %}{{ post.content | strip_html | strip_newlines | truncate: 120 }}{% endif %}</p>
  {% endfor %}
 </article>
</div>