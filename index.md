---
layout: default
description: "Resumo da vida acadêmica, profissional e pessoal de Fabio Nobre."
---
{% if page.language == "en" %}{% assign data = site.data.dataen %}{% else %}{% assign data = site.data.data %}{% endif %}{% include title.html %}
{% include career-profile.html %} 
{% include experiences.html %}
{% unless data.sidebar.education %}
{% include education.html %}
{% endunless %}
{% include projects.html %}
{% include publications.html %}
