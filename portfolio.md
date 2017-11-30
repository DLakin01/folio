---
layout: page
title: portfolio
permalink: /portfolio/
---

{% for project in site.portfolio %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>

        </span>
        </a>
        <h1>{{ project.title }}</h1>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>

        </span>
        </a>
        <h1>{{ project.title }}</h1>
    </div>
</div>

{% endif %}

{% endfor %}

<h4 class="post-content">
See the code for these projects and more on my
<a href="https://github.com/DLakin01">GitHub.</a>
</h4>
