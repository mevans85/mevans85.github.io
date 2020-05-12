---
layout: default
permalink: /write-ups/
---

Welcome to the Write-Ups! Please navigate the posts accordingly..

<section class="posts">

<ul>
{% for category in site.categories %}
{% if category[0] == "Write-Up" or  category[0] == "writeup" or  category[0] == "Writeup" or  category[0] == "write-up" or  category[0] == "WRITEUP" or  category[0] == "WRITE-UP" or category[0] == "Write-Ups" %}
{% for post in category[1] %}
<li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time></li>
{% endfor %}
{% endif %}
{% endfor %}
</ul>

</section>

