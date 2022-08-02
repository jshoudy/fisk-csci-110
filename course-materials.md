---
layout: page
title: Course Materials
description: Listing of course modules and topics.
---

# Course Materials
This calendar outlines all topics of the course and has links to all slides and assignments.

{% for module in site.modules %}
{{ module }}
{% endfor %}

