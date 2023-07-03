---
layout: page
title: Resume
permalink: /resume/
---

<br>

<h2>Experience</h2>
{%- for experience in site.categories.experience -%}
<ul>
    <li>
        <h3> {{ experience.position }} at {{ experience.company }} </h3>
        <h4> from {{ experience.startdate }} to {{ experience.enddate }} in {{ experience.location }}</h4>
        {{ experience.content }}
    </li>
</ul>
{%- endfor -%}

<br>

<h2>Education</h2>
{%- for education in site.categories.education -%}
<ul>
    <li>
        <h3> {{ education.award }} at {{ education.school }} </h3>
        <h4> in {{ education.location }}</h4>
    </li>
</ul>
{%- endfor -%}

<br>

<h2>Skills</h2>
{%- for skills in site.categories.skills -%}
<ul>
    <li>
        <h3> {{ skills.title }} </h3>
        <h4> {{ skills.content }}</h4>
    </li>
</ul>
{%- endfor -%}

<br>

<h2>Certfications</h2>
{%- for certifications in site.categories.certifications -%}
<ul>
    <li>
        <h3> {{ certifications.title }} of {{ certifications.course }} from {{ certifications.source }} </h3>
        <h4> {{ certifications.content }}</h4>
    </li>
</ul>
{%- endfor -%}