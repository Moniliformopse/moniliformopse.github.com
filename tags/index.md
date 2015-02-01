---
layout: page
title: Tag Index
excerpt: "An archive of posts sorted by tag."
search_omit: true
---

{% capture site_tags %}{% for tag in site.tags %}{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
{% assign tags_list = site_tags | split:',' | sort %}

<ul class="tag-box inline">
  {% for item in (0..site.tags.size) %}{% unless forloop.last %}
    {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
    <li><a href="#{{ this_word }}">{{ this_word }} <span>{{ site.tags[this_word].size }}</span></a></li>
  {% endunless %}{% endfor %}
</ul>

{% for item in (0..site.tags.size) %}{% unless forloop.last %}
  {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
  <h2 id="{{ this_word }}">{{ this_word }}</h2>
  <ul class="post-list">
  {% for post in site.tags[this_word] %}{% if post.title != null %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}<span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{% assign d = post.date | date: "%-d"  %}{% case d %}{% when '1' %}{{ d }}er{% else %}{{ d }}{% endcase %} {% assign m = post.date | date: "%-m" %}{% case m %}{% when '1' %}janv.{% when '2' %}févr.{% when '3' %}mars{% when '4' %}avr.{% when '5' %}mai{% when '6' %}juin{% when '7' %}juil.{% when '8' %}août{% when '9' %}sept.{% when '10' %}oct.{% when '11' %}nov.{% when '12' %}déc.{% endcase %} {{ post.date | date: '%Y' }}</time></span></a></li>
  {% endif %}{% endfor %}
  </ul>
{% endunless %}{% endfor %}