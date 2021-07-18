title: Online Hosted Instructions
permalink: index.html
layout: home

# Content Directory

Required labs files can be [DOWNLOADED HERE](https://github.com/AceTheCloud/AZ-104.github.io/archive/master.zip)

## Labs

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| Module | Lab |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

All Labs Prepared by Microsoft and Microsoft Learn Community