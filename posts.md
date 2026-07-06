---
layout: default
title: "posts"
---

<h1 style="text-align: center;"> Post Board </h1>

___

<div class="post_board">
    {% for post in site.posts %}
        {% include postcard.html title=post.title excerpt=post.excerpt date=post.date url=post.url %}
    {% endfor %}
</div>

___