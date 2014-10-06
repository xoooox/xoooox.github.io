---
layout: page
title: Performativas
published: True
---

<hr>
{% assign pages_list = site.performativas %}
{% for node in pages_list %}
{% if node.title != null %}
<div class="entry">
<!--<div class="posts">-->
<hr>
<div class="entry-content">
<h2 class="entry-title">
<!--<a class="white" href="{{ post.url }}"><span class="icon icon-forward entry-icon"></span>{{ post.title }}</a>-->
<a class="entry-thumb" href="{{ node.url }}" title="Visit {{ node.title }}" target="_blank">
<span class="icon icon-forward entry-icon"></span>
{{ node.title }}
</a>
  
</h2>
</div>

{{ node.content }}

<a class="entry-thumb" href="{{ post.url }}" title="Visit {{ post.title }}" target="_blank">
<span class="icon icon-forward entry-icon"></span>
</a>
<div class="entry-content">
<!--<h2 class="entry-title">
<a href="{{ post.url }}">{{ post.title }}</a>
</h2>-->
<p class="entry-date">{{ post.date | date: "%B %-d, %Y" }}</p>
</div>
</div>
<hr>
{% endif %}
{% endfor %}

<hr>




{% include pagination.html %}
