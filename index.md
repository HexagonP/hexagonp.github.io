---
layout: default
title: "home"
excerpt: "page of a fox"
---

<img style="float: right;" alt="fob" src="/assets/images/fob.png">
## WELCOME
this website is still being worked on, but in the meantime you can check these out:

{% include button_a.html icon="/assets/icons/like.png" text="games i like" url="https://hexagonp2.carrd.co" %}
{% include button_a.html icon="/assets/icons/games.png" text="my itch.io page" url="https://hexagonp.itch.io" %}
{% include button_a.html icon="/assets/icons/music.png" text="music stuff" url="https://www.youtube.com/@hexscendo" %}
{% include button_a.html icon="/assets/icons/what.png" text="mystery button" url="https://youtu.be/yPYZpwSpKmA" %}

<h1 style="text-align: center; margin-top: 64px;"> Latest Posts </h1>
___

<div class="post_board">
    {% for post in site.posts limit:3 %}
        {% include postcard.html title=post.title excerpt=post.excerpt date=post.date url=post.url %}
    {% endfor %}
</div>

___