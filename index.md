---
layout: page
title: 
tagline: Supporting tagline
---
{% include JB/setup %}

<ul class="posts">
{% for post in site.posts %}
    	<br>
	<a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}
	</a> 
		&raquo; 
		<span>
		{{ post.date | date_to_string }}
		</span> 
	</br>
    	<li>
		<span>
		{{ post.content }}
		</span>
	</li>
  {% endfor %}
</ul>

