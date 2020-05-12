---
layout: default
permalink: /blog/
---

Welcome to the blog! Please navigate the posts accordingly..

<section class="posts">
<ul>
{% for category in site.categories %}
{% if category[0] == "Blog" or category[0] == "blog" or category[0] == "BLOG" %}
{% for post in category[1] %}
<li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time></li>
{% endfor %}
{% endif %}
{% endfor %}
</ul>
</section>

