---
layout: default
title: Publications
permalink: /publications/
---

<h1>Publications</h1>

<div class="publications-list">
    {% assign all_publications = site.publications | sort: 'date' | reverse %}

    {% if all_publications.size > 0 %}
        {% for item in all_publications %}
            {% include widgets/publication_item.html item=item %}
        {% endfor %}
    {% else %}
        <p>No publications available.</p>
    {% endif %}
</div>
