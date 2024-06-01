{% for p in site.posts %}
  [{{ p.title }}]({{ site.baseurl }}{{ p.url }})
  {% for cat in p.categories %}
    {% if cat == "tech"}
      ![Technology](https://img.shields.io/badge/-Tech-0078d7?style=flat)
    {% endif%}
    {% if cat == "cybersecurity"}
      ![Cybersecurity](https://img.shields.io/badge/-Cybersecurity-000000?style=flat)
    {% endif%}

  {% endfor %}
{% endfor %}