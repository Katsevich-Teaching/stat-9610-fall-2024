---
layout: page
title: Staff
description: A listing of all the course staff members.
nav_order: 8
---

# Staff

## Instructor

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}

## Teaching Assistant

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
