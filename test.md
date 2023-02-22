---
layout: page
---

# Test

{% for collection in site.collections %}

  ## {{ collection.label }}

  <ul>
    {% for doc in collection.docs %}
      <li><a href="{{ doc.url }}">{{ doc.title }}</a></li>
    {% endfor %}
  </ul>

{% endfor %}
