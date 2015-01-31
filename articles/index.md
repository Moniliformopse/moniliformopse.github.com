---
layout: page
title: Archives
excerpt: "An archive of posts sorted by date."
search_omit: true
---

<ul class="post-list">
{% for post in site.categories.articles %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{% assign d = post.date | date: "%-d"  %}{% case d %}{% when '1' %}{{ d }}er{% else %}{{ d }}{% endcase %} {% assign m = post.date | date: "%-m" %}{% case m %}{% when '1' %}janv.{% when '2' %}févr.{% when '3' %}mars{% when '4' %}avr.{% when '5' %}mai{% when '6' %}juin{% when '7' %}juil.{% when '8' %}août{% when '9' %}sept.{% when '10' %}oct.{% when '11' %}nov.{% when '12' %}déc.{% endcase %} {{ post.date | date: '%Y' }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
