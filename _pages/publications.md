---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
<div class="amtText" markdown="1">
*Note: if you don't have access to any of the journals where my publication links lead you, or I haven't yet made a link active, please just email me to get a copy.*
</div>

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% assign items = site.publications | sort: 'date' %}

{% for post in items reversed %}
  {% if (post.publicationText %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

{% for post in items reversed %}
  {% if (post.publicationText %}
    {% assign goober = "Done already" %}
  {% else %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
