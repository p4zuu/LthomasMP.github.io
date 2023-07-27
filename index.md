---
layout: default
title: Homepage
---

<h1>Posts</h1>
<ul class="posts">
    {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span>: <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>

<h1>Findings</h1>
<ul class="bugs">
    {% for bug in site.data.bugs.bugs %}
    <li><span>{{ bug.package }}</span>: <a href="{{ bug.url }}" title="{{ bug.title }}">{{ bug.title }}</a></li>
    {% endfor %}
</ul>
