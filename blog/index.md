{% for post in site.posts limit:5 %}  

  <div class="card text-white bg-dark">
    <div class="card-body">
      <h5 class="card-title"><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h5>
      {% for cat in post.categories %}
        <a href="{{ BASE_PATH }}{{ cat.url }}" class="badge badge-primary">{{ cat }}</a>
      {% endfor %}
      {% if post.excerpt %}
        <p class="card-text">{{ post.excerpt }}</p>
      {% endif %}
      <a href="{{ BASE_PATH }}{{ post.url }}" class="btn btn-primary">Read more</a>
        
    </div>
  </div>
{% endfor %}  