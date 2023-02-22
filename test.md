---
layout: page
---

# Test

{% for collection in site.collections %}
  {% if collection.label != "posts" %}
<h2><a href="#">{{ collection.title }}</a></h2>
<ul>
    {% for doc in collection.docs %}
<li><a href="{{ doc.url }}">{{ doc.title }}</a></li>
    {% endfor %}
</ul>
  {% endif %}
{% endfor %}
