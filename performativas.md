---
layout: page
title: Performativas
published: True
---
<hr>
<ul>
{% assign pages_list = site.performativas %}
{% for node in pages_list %}
{% if node.title != null %}

<li class="nav-item">
<a class="nav-link{% if page.url == node.url %} nav-link-active{% endif %}" href="{{ node.url }}">{{ node.title }}</a>
</li>

node.output

{% endif %}
{% endfor %}
</ul>
<hr>
