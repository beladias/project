---
layout: work
title: Work
---

<h1>{{ page.title }}</h1>

<h2>Projects I've been working in the past year</h2>

<ul>
    {% for project in site.data.work %}
        <hr>
        <li class="worklist">
            <a href="{{ site.baseurl }}{{ project.perma }}"> 
            {{ project.title }}
            <figure>
                <img src="{{ site.baseurl }}{{ project.img }}" alt="{{ project.image-alt }}" title="{{ project.image-alt }}">
            </figure>
            </a>
        </li>
    {% endfor %}
</ul>