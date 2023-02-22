---
layout: page
---

# Test

{% for collection in site.collections %}

  <h2><a href="{{ collection.directory }}">{{ collection.label }}</a></h2>

  <ul>
    {% for doc in collection.docs %}
      <li><a href="{{ doc.url }}">{{ doc.title }}</a></li>
    {% endfor %}
  </ul>

{% endfor %}
