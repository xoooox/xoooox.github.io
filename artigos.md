---
layout: page
title: Artigos
published: true
---
<hr>
{% assign pages_list = site.artigos %}
{% for node in pages_list %}
{% if node.title != null %}

<li class="nav-item">
<a class="nav-link{% if page.url == node.url %} nav-link-active{% endif %}" href="{{ node.url }}">{{ node.title }}</a>
</li>


{% endif %}
{% endfor %}
<hr>

Artigos sobre merdas, e artigos de merda, tudo junto num só texto

Tanta merda junto, tem que produzir energia

Às escuras ninguém fica

Com cheiro amarelo dos artigos.







```
rui.felizes@oocn.eu {MMXIV}
```

