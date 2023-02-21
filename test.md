---
layout: page
---

# Test

<ul>
{% for general in site.general %}
  <li>
    <a href="{{ general.url }}">
      {{ general.title }}
    </a>
  </li>
{% endfor %}
</ul>
