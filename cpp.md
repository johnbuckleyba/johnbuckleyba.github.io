---
layout: page
title: Commercial Photographic Practise
permalink: /cpp/
---

{% for project in site.cpp %}
<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h3>{{ project.title }}</h3>
            <br/>
            <h4>{{ project.description }}</h4>
        </span>
        </a>
    </div>
</div>

{% endfor %}
