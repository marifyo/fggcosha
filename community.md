---
layout: page
permalink: /community/
title: Community
---

## Spotlights
<div>
 {% for pc in page.categories %}
 {% if pc == "spotlight" %}
 	{% for post in site.categories.spotlight %}
	    {% if page.title != post.title %}   
	    <article>
    	 <h2><a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></h2>
    	</article>
         {% endif %}
    {% endfor %}
  {% endif %}
  {% endfor %}
</div>