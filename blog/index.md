---
layout: page
title: Scott Chamberlain's Lab Notebook
---

<div id="posts">
  <h1>Blog posts</h1>
    {% for post in site.posts %}
		<code>{{ post.date | date_to_string }}</code> » <span class='post-title'><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></span><br /><span class='meta'>Tags: {% for tag in post.tags %}{{ tag | array_to_sentence_string }}{% endfor %}</span><p />
    {% endfor %}
</div>