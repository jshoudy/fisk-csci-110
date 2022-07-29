---
layout: page
title: Staff
description: A listing of all the course staff members.
---

# Staff

For a quicker response on homework or project help, please ask on [Piazza](https://piazza.com/fisk/fall2022/csci110/home) rather than emailing staff members individually. On Piazza, all staff members can see your question and answer it.

## Instructors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign fisk_teaching_assistants = site.staffers | where: 'role', 'Fisk Teaching Assistant' %}
{% assign num_fisk_teaching_assistants = fisk_teaching_assistants | size %}
{% if num_fisk_teaching_assistants != 0 %}
## Fisk Teaching Assistants

{% for staffer in fisk_teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign google_teaching_assistants = site.staffers | where: 'role', 'Google Teaching Assistant' %}
{% assign num_google_teaching_assistants = google_teaching_assistants | size %}
{% if num_google_teaching_assistants != 0 %}
## Google Teaching Assistants

{% for staffer in google_teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
