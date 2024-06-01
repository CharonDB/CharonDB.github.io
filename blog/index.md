{% for p in site.posts %}
  [{{ p.title }}]({{ site.baseurl }}{{ p.url }})
  {{ p.categories }}
{% endfor %}