---
layout: default
permalink: /
---

## Welcome

<img class="profile-picture" src="assets/images/hacker.jpg" alt="Hacker">

Hello and welcome to the <i><b>I Hack Stuff</b></i> web site.  I have created this site as a platform to document my ongoing learning and research.  By documenting, it allows me to solidify the knowledge and also helps others.  It is also a central place for all my contact information and my basic online presence.  

Please check the <a href="/about">about</a> section to find out more detailed information.



## Recent Posts

<div> 
The following are the five most recent posts:

	<table>
		<tr>
			<th>Date</th>
			<th>Category</th>
			<th>Posts</th>
		</tr>
		{% for post in site.posts limit:5 %}
			<tr>
			<td>{{ post.date | date_to_string}}</td>
			<td>
				{% if post.category == "Blog" or post.category == "blog" %}
				 Blog Post
				{% else %}
				{{ post.category }}
				{% endif %}
			</td>
			<td><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a><br></td>	
			</tr>
		{% endfor %}
	</table>

</div>
