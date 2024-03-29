---
layout: home
title: Proofs and programs
nav_exclude: true
seo:
  type: Course
  name: Intro to Proofs
---

# {% if site.honors %} HNRS: {% endif %} {{ site.tagline }}
{: .mb-2 }
{{ site.description }}
{: .fs-6 .fw-300 }

{% if site.announcements %}
{% for announcement in site.announcements %}
{% assign announce_date = announcement.date | date: '%s' | times: 1 %}
{% assign announce_date_plus_week = announce_date | plus: 604800 %}
{% assign today_date = 'now' | date: '%s' | times: 1 %}
{% if announce_date <= today_date and announce_date_plus_week > today_date %}
{{ site.announcements.first }}
[Announcements]({% link announcements.md %}){: .btn .btn-outline .fs-3 }
{% endif %}
{% endfor %}
{% endif %}

## Syllabus 

The syllabus can be found at the [syllabus tab]({% link syllabus.md %}). 

## Calendar 

At the [calendar tab]({% link calendar.md %}), you will find our topic schedule 
for each class along with the pre-reading, worksheets for that class, and 
due dates for assignments.  

## Notes 

Notes can be found in their [GitHub repository](https://github.com/UofSC-Spring-2023-SCHC-411-H01/notes/). 

## Homework

There are tabs for class [homework]({% link homework/index.md %}). 

Homework is turned in weekly and in groups of 3-4. 

For more information, see the [Syllabus]({% link syllabus.md %}).

## Me

If you are interested in a bit about who I am and what I do, check out the 
[staff tab]({% link staff.md %}) or visit [my website](https://www.matthewrobertballard.com).
