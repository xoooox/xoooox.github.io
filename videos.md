---
layout: page
title: Videos
published: true
---
<hr>
{% assign pages_list = site.video %}
{% for node in pages_list %}
{% if node.title != null %}

<li class="nav-item">
<a class="nav-link{% if page.url == node.url %} nav-link-active{% endif %}" href="{{ node.url }}">{{ node.title }}</a>
</li>


{% endif %}
{% endfor %}
<hr>




```
rui.felizes@oocn.eu {MMXIV}
```

