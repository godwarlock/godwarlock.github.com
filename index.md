---
layout: page
title: GODSHARE 
tagline: Supporting tagline
---
{% include JB/setup %}

<ul class="posts">
{% for post in site.posts %}
	<h1>
    	<br>
		<a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}
		</a> 
		&raquo; 
		<span>
		{{ post.date | date:"%B %d, %Y" }}
		</span> 
	</br>
	</h1>
    	<br>
		<span>
		{{ post.content }}
		</span>
	</br>
  {% endfor %}
</ul>

