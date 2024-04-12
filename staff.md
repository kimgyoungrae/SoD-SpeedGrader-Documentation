---
layout: page
title: Support Staff
description: A listing of all the course staff members.
---

# Support Staff
## Student Assistant

{% assign instructors = site.staffers | where: 'role', 'Student Assistant' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}





{% assign teaching_assistants = site.staffers | where: 'role', 'Program Coordinator' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Program Coodinators

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
