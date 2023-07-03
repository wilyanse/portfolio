---
layout: page
title: Projects
permalink: /projects/
---

{%- for projects in site.categories.projects -%}
<ul>
    <li>
        <h3> <a href="{{ projects.url | relative_url }}"> {{ projects.title }} </a> </h3>
        <h4> {{ projects.shortdes }} </h4>
        <h5><a href="{{ projects.link }}"> Github Link </a></h5>
    </li>
</ul>
{%- endfor -%}