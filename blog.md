---
layout: default
title: 博文
---

<div>
    <h1 class="post_title">博文</h1>
    <div class="post_list">
        {% for post in site.posts %}
        {% if post.display == "onlydetail" %}
        {% else %}
        <a class="post_list_item" href="{{ post.url }}">
            {{ post.date | date_to_string }}
            &raquo; 
            {{ post.title }}
        </a>
        {% endif %}
        {% endfor %}
    </div>
</div>

