---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

*Note: if you don't have access to any of the journals where my publication links lead you, or I haven't yet made a link active, please just email me to get a copy.*

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
