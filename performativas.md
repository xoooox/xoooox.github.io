---
layout: Page
title: Performativas
---


{% assign pages_list = site.performativas %}
{% for node in pages_list %}
<div class="entry">
<!--<div class="posts">-->
<hr>
<div class="entry-content">
<h2 class="entry-title">
<!--<a class="white" href="{{ node.url }}"><span class="icon icon-forward entry-icon"></span>{{ node.title }}</a>-->
<a class="entry-thumb" href="{{ node.url }}" title="Visit {{ node.title }}" target="_blank">
<span class="icon icon-forward entry-icon"></span>
{{ node.title }}
</a>
  
</h2>
</div>
<!--<div class="post"><h2 class="post-title"><a class="white" href="{{ post.url }}">{{ post.title }}</a></h2></div>-->

{{ node.excerpt }}

<a class="entry-thumb" href="{{ node.url }}" title="Visit {{ node.title }}" target="_blank">
<span class="icon icon-forward entry-icon"></span>
</a>
<div class="entry-content">
<!--<h2 class="entry-title">
<a href="{{ node.url }}">{{ node.title }}</a>
</h2>-->
<p class="entry-date">{{ node.date | date: "%B %-d, %Y" }}</p>
</div>
</div>
<hr>
{% endfor %}

{% include pagination.html %}
