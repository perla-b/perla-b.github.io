---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<ul>
{% for post in site.posts reversed limit:5 %}
	<a href="{{ post.url }}">
	<h2>
		{{ post.title }}
	</h2>
	</a>
	<p>
		{{ post.content }}
	</p>
	<hr>
{% endfor %}
</ul>

